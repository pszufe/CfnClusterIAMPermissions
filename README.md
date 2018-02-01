# CfnCluster Super Quick Start

Working with the AWS CfnCluster I found out that the most difficult issue for non AWS-expert computational scientists is to properly configure all security settings to have a working, useful cluster with a place to store data. I decided to fill-in this gap and publish the script below.

This AWS Cloud Formation script creates 
- AWS IAM Security settings for a CfnCluster management instance
- AWS IAM Security settings for a CfnCluster node (this settings can be passed by the management instance)
- an S3 bucket along with relevant permission that can be used to store CfnCluster computations 

[click this link to launch the script](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/create/review?templateURL=https://raw.githubusercontent.com/pszufe/CfnClusterIAMPermissions/master/CfnCluster.json&stackName=CfnCluster)
The link will only work while being logged-in to your AWS account. Select the checkbox *I acknowledge that AWS CloudFormation might create IAM resources.*, click *Create*, wait 4 minutes and you are done.



