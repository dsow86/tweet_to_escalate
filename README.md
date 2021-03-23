# tweet_to_escalate
In this model, we help Naomi identify which tweets should be escalated to her support
team and which tweets could be handled by an automated bot and provide a way for her to send tweets to the machine
learning model and receive a decision as to whether a tweet should be escalated.
The data containing the tweets cand be find here:
We use boto3, the python sdk for aws, to connect locally from aws interface, create a bucket, define policies and upload data on it. 
We use the SageMaker endpoint to serve predictions to an API on aws lambda using the chalice python package.
To access the SageMaker endpoint, our serverless API needs to have permission to do so. Using Microsoft’s Visual Studio Code (VS Code), you set up credentials in our AWS account by creating an access key, then setting up our
AWS credentials on our local computer.
