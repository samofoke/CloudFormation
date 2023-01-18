# CloudFormation

- We will have this as our header AWSTemplateFormatVersion	"2010-09-09".
- Then have the description of our Cloudformation script.
- This is our command for creating a CloudFormation Script via the AWS CLI.
    ~~~
    aws cloudformation create-stack --stack-name myFirstVpcTest02 --region us-east-1 --template-body file://[Name of the Stack]
    ~~~
- We can also update the Stack yo the existing deployed stack to avoid any errors.
    ~~~
    aws cloudformation update-stack  --stack-name myFirstTest --region us-east-1 --template-body file://[Name of the Stack]

    ~~~
- We also have this command for describing the stack.
    ~~~
    aws cloudformation describe-stacks --stack-name [Name of the stack]
    ~~~
- 