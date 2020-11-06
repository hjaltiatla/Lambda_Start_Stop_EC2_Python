# Lambda Scripts to start and Stop AWS EC2 Instances 

#### Steps to setup Execution Role via AWS web console to allow the Lambda function to have execution permission via the EC2 instances

1. IAM >> CREATE Role
1. Create Policy >> JSON >> Copy lambdarole.json text to the JSON Text field >> Review Policy
1. Name the Policy "lamdastartstop" >> Create policy >> Attatch the policy to the new role
1. Next >> Next >> Role Name = "Ec2StartStopLambdaRole" >> Create Role


#### After Creating the Lambda Functions you need to add an Environment variable for the functions with the Ec2 instance ID
Key= "EC2_INSTANCES"
Value= "instance ID"
([Instance ID Example](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/images/clearbox-view-ec2-instances-3.png))

