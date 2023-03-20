# akm-cloud-security-assessment-permission-templates-public
Templates that create needed IAM Role in an AWS account to be scanned by AKM Enterprises OÜ Assessment team.


# For AWS Cloud Security Assessment, engage us through Fiverr - https://www.fiverr.com/s2/a7aed84e2c

## In order to conduct security assessment of your account AKM security assessment IAM role need access to your AWS account. 

## This ‘create_role_to_assume_cfn.yaml’ cloudformation template will create the rule and trust AKM AWS account’s security assessment role
This cloudformation can be deployed through AWS console or AWS cli

AWS CLI 

'''sh
# aws cloudformation create-stack \
#  --capabilities CAPABILITY_IAM --capabilities CAPABILITY_NAMED_IAM \
#  --template-body "file://create_role_to_assume_cfn.yaml" \
#  --stack-name "ProwlerScanRole_for_AKM" \
#  --parameters "ParameterKey=AuthorisedARN,ParameterValue=arn:aws:iam::080817114978:role/akm_security_assessment_role"
#
'''

