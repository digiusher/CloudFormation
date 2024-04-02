# AWS CloudFormation Stack Creation

This README provides instructions on how to create a CloudFormation stack using the provided templates and how to upload and execute these scripts in your AWS environment.

This repository contains two CloudFormation templates: `CloudFormationWithCur` and `CloudFormationWithoutCur`. The purpose of these templates is to provision AWS resources automatically based on specific requirements.

These templates are designed to cater to different scenarios: one with CUR enabled and one without CUR enabled. By using these templates, you can ensure that the required infrastructure is provisioned correctly based on your specific needs.

## Instructions

1. **Download the Templates**:
   Clone this repository or download the CloudFormation templates `CloudFormationWithCur.yaml` and `CloudFormationWithoutCur.yaml`.

2. **Choose Template**:
   Depending on whether you have Cost and Usage Reports (CUR) enabled or not in your AWS account, choose the appropriate CloudFormation template:
   - If CUR is enabled, use `CloudFormationWithCur.yaml`.
   - If CUR is not enabled, use `CloudFormationWithoutCur.yaml`.

3. **Create CloudFormation Stack**:
   Use the AWS Management Console to create a CloudFormation stack:
   - Go to the CloudFormation service in the AWS Management Console.
   - Click on "Create stack" and choose "With new resources (standard)".
   - Select "Upload a template file" and upload the choosen template.
   - Follow the on-screen instructions to specify stack details, skip configuring stack options, and create the stack.

4. **Monitor Stack Creation**:
   Monitor the stack creation process through the AWS Management Console.

5. **Navigate to Outputs**:
   After the stack creation is complete, navigate to the "Outputs" section in the CloudFormation stack details.

6. **Fill in Output Values**:
   Use the output values provided and fill them in the fields when connecting to the AWS ARN data source.
