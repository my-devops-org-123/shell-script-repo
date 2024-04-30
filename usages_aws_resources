###########
#Author: amrita
#Date: 30 Apr
#version: v1
#This script will report the AWS resources usages

set -x
# list s3 bucket
echo "pring list of s3 bucket"
aws s3 ls > shell2.sh

# list of ec2 instance
echo "pring list of ec2 instance"
aws ec2 describe-instances | jq '.Reservations[].Instances[].InstanceId' > shell2.sh

# list of lambda-function
echo "pring list of lambda function"
aws lambda list-functions > shell2.sh

# list of IAM users
echo "pring list IAM user"
aws iam list-users > shell2.sh
