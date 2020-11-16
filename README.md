# file-UploaderService-esp-home123

Project – Uploading images to AWS S3 with Serverless using AWS Lambda

Overview:
 

Tools Required:

•	AWS CLI

•	NodeJS 12

•	Serverless

1.	Install AWS CLI(Command Line Interface)

    export AWS_ACCESS_KEY_ID=*****************

    export AWS_SECRET_ACCESS_KEY=*************************************

2.	Install the NodeJS and serverless framework

    •	Install module: sudo npm install -g serverless@beta

    •	Create project directory: mkdir file-UploaderService-esp-home123; cd mkdir file-UploaderService-esp-home123

3.	Run the following command to generate sample code with serverless

    Serverless create –template aws-nodejs

    The above command will create the following files:
    
    •	serverless.yml
    
    •	handler.js

4.	Install dependencies

    •	npm init -y

    •	npm install busboy && uuid && jimp && aws-sdk

    •	npm install jimp uuid

5.	Create the function to decode the form-data

    formParser.js //code available over github

6.	Function that will process and upload the images to S3: rename handler.js to fileUploaderHome.js and make all changes

7.	Edit the serverless.yml

8.	We have finished with all the services now deploy the service using below command

    •	serverless deploy or sls deploy --stage=test

Now test this post url using postman and check logs on aws

9.	Postman test

10.	Lambda monitoring & Log output

11.	To Remove the Service run below command

    sls remove --stage=test
