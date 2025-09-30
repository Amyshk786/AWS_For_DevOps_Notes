Day-15 | AWS ULTIMATE CICD PIPELINE | END TO END DEMO | AWS CODE PIPELINE
==========================================================================


- Go to AWS Code Deploy  -> Create Application & Name [sample-python-flask-app]  & Compute Platform as EC2


- Create an EC2 Instance with the name python-flask-app   [Provide Tag as Name python-flask-app]


- Now we have to Install Agent on the EC2 Instance which we have Created


- LogIn to the Instance and Follow the Below Mentioned Documentation 


Link - https://docs.aws.amazon.com/codedeploy/latest/userguide/codedeploy-agent-operations-install-ubuntu.html

Region Name Link - https://docs.aws.amazon.com/codedeploy/latest/userguide/resource-kit.html#resource-kit-bucket-names



 sudo apt-get update 
 
 sudo apt install ruby-full

 sudo apt install wget

 wget https://aws-codedeploy-us-east-1.s3.us-east-1.amazonaws.com/latest/install

 chmod +x ./install

 sudo ./install auto

 sudo systemctl status codedeploy-agent 



- Now we will go to IAM and Create a Role so that the EC2 Instance and the CodeDeploy can talk to Each Other


- EC2 CodeDeploy role and Attach the role to the Instance

 EC2 Instance Settings -> Security -> Modify IAM Role  [If this is not working use below command]


1. aws iam create-instance-profile --instance-profile-name ec2-codedeploy-role-profile

2. aws iam add-role-to-instance-profile --instance-profile-name ec2-codedeploy-role-profile --role-name ec2-codedeploy-role 

3. aws ec2 associate-iam-instance-profile --instance-id i-0123456789abcdef0 --iam-instance-profile Name=ec2-codedeploy-role-profile




# Now we will Configure CodeDeploy


- Go to Applications -> Create Deployment Group -> Name= python-flask-app -> Select the Role


- Select EC2 Instance and Add the tag which we have given to our Instance


- Un-Check the Load Balancing Option and Click on Create Deployment Group 




# Now Comes the Final Step where we will be Creating a Deployment and for this we will require appspec.yml


- Provide the Deployment Group -> My App is on GitHub -> Provide Authorization to GitHub


- Provide the repo name "https://github.com/Amyshk786/aws-devops-zero-to-hero"


- Provide the Commit ID "81a7ceb"  & Click on Create Deployment






