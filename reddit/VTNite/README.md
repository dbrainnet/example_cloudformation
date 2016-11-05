# Helping /u/VTNite on reddit
These templates are for public consumption, in particular I'm aiming to help /u/VTNite on reddit get started in CloudFormation
Link to help request for context: https://www.reddit.com/r/aws/comments/5b6vxa/cloudformation_help/

# Purpose
This template is for education, learning and understanding purposes only, it is very far from best practice. The purpose of this template is to help someone get started and achieve a goal quickly with a limited example. 

# Usage
This template comes with out any warranty.

AWS charges will be incurred by using this template and by using this template the user agrees to pay AWS for the services used. 

When using this template you will be asked to provide parameter values for the following:

| Parameter Name | Expected Value |
| -------------- | -------------- |
| AMI1 | AMI Id to use for the first AutoScaling Group, you have to supply this string on your own |
| AMI2 | AMI Id to use for the second AutoScaling Group, you have to supply this string on your own |
| EC2KeyPair | A EC2 KeyPair Name used for both ASG's, when booting through the console you will be prompted with a drop down |
| InstanceType | Instance Type size to use for instances in both ASG's, when booting through the console you will be prompted with a drop down |
| MaxInstanceCount | Maximum number of instances in each ASG, must be larger than MinInstanceCount, you must supply integer altho there is a default |
| MinInstanceCount | Minimum number of instances in each ASG, must be smaller than MaxInstanceCount, you must supply integer altho there is a default |
| SecurityGroups | A list of security groups, these must be in the same VPC as the subnets, used for both ASG's, when booting through the console you will be prompted with a drop down |
| Subnets | A list of subnet Id's these must be in the same VPC, used for both ASG's, when booting through the console you will be prompted with a drop down |
