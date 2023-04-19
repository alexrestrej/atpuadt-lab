# atpuadt-lab
Advanced Testing Practices Using AWS DevOps Tools available on AWS Sikll Builder.

Link to course: https://explore.skillbuilder.aws/learn/course/5741/play;state=%5Bobject%20Object%5D;autoplay=0

# Creating sandbox environment

The stack creation will take about 15 minutes to build. When it is complete, navigate to CodePipeline in the AWS console to view the resources that are created.
Note: Remember to terminate resources when you have finished using them to avoid incurring additional charges.

1. At this point, you should have already downloaded the zip file that was provided. If not, please do so before proceeding.
2. Unzip the demoEnv.zip file to your local machine.
3. Log in to the AWS console for your account and navigate to Amazon S3.
4. Create a new S3 bucket in the Region you wish to deploy the template.
5. Copy the contents of the zip file to the S3 bucket. There should be three files: functions.zip, cicd.template and calculator.zip
6. Navigate to AWS CloudFormation and choose Create Stack (with new resources Standard).
7. In the Template is Ready section, provide the link to the cicd.template from your S3 bucket.
8. Choose Next. Enter the stack name and provide the bucket name for where the functions.zip and calculator.zip files are stored.
9. Choose Next twice. Then select that you acknowledge the template will create resources.
10. Choose Create Stack.  

# Resolving challenges

## Challenge 1

View the release pipeline’s progress and note the completed and pending stages. Then, review the resolved configuration settings of the Service_Status stage. Access the deployed sample application using the URL.

## Challenge 2

The release pipeline is currently pending for approval. Approve or reject the stage action Purge_Test and notice how your pipeline reacts.

## Challenge 3

Evaluate the provided sample code using Cloud9 IDE. In the application.json file, change the security group definition to 0.0.0.0/0. Then, commit your changes to the repository using Cloud9 IDE. Observe how your pipeline reacts.

## Challenge 4

Perform a pull request and a review for the sample application code change.

## Challenge 5

Review the Service_Stage in the release pipeline to understand how the synthetic testing was set up. Make the code changes to index.html to fail the testing








