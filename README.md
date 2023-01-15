# CloudFormation

- We will have this as our header AWSTemplateFormatVersion	"2010-09-09".
- Then have the description of our Cloudformation script.
- This is our command for creating a CloudFormation Script via the AWS CLI.
    ~~~
    aws cloudformation create-stack --stack-name myFirstVpcTest02 --region us-east-1 --template-body file://CloudFormation-Script.yaml
    ~~~
- 