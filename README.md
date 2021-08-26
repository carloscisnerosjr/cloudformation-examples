# Cloudformation Example

This repository contains an example of a Cloudformation template. Deploying this will allow an AWS SysOps Adminsitrator manage the lifecycle of AWS Workspaces using a AWS Systems Manager maintenance schedule, S3 and Lambda. A CSV file of a current list of AD users is generated that is then used to compare to a list of current users in AWS Workspaces. If the user is present in the AD user list but not in the WorkSpaces list, the Workspace is terminated. If user is present in WorkSpaces list but not in AD user list, the Workspace is terminated. The Python code uses the csv,logging, os and boto modules. The Powershell code users the Get-ADUser cmdlet. 

