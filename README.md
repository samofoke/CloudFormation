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
- We also need this commands before we run our aws cli
    ~~~
    aws configure
    aws iam list-users to list users we have.
    {
    "Users": [
        {
            "Path": "/",
            "UserName": "Dev",
            "UserId": "User ID key",
            "Arn": "arn:aws:iam::[numbers]:user/Dev",
            "CreateDate": "The date it was created"
        }
      ]
    }
    ~~~
- When you add a DependsOn attribute to a resource, that resource is created only after the creation of the resource specified in the DependsOn attribute.
    ~~~
    "DependsOn" : [ String, ... ]
    ~~~
- We also have the !GetAtt function it returns the value of an attribute from a resource in the template.
    ~~~
    !GetAtt logicalNameOfResource.attributeName
    ~~~
- Route Tables it is an action of applying (routing) rules to your network, rules define (in a particular order of precedence) the network protocol, allowed IP addresses, and ports to allow the inbound and outbound traffic separately.
    ~~~
    This will be defined as AWS::EC2::RouteTable on our CloudFormation Script.
    Rules will be AWS::EC2::Route 
    ~~~
- 