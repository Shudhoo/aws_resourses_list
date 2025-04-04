
# AWS Resources List Script

So, hi everyone! This is my learning journey of Linux OS and Linux fundamentals. However, this script mainly focuses on shell scripting, which is highly important in a DevOps & Cloud Engineer’s daily tasks.

This script helps you list AWS services running on your account, whether it's EC2, S3, RDS, Lambda, etc. It saves time by eliminating the need to manually check running resources and generate reports. Instead of running multiple AWS CLI commands, this script provides all the necessary information in one place.

### Prerequisites

Before running this script, ensure the following are set up:

1.) Install AWS CLI using the following commands:

```bash
  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
  unzip awscliv2.zip
  sudo ./aws/install
```
2.) Configure AWS CLI using the following command:

```bash
   aws configure
```

For reference visit AWS CLI https://docs.aws.amazon.com/streams/latest/dev/setup-awscli.html

After completing all these installations and configurations, you are all set to run this script on your system.

However, remember that this script can only be executed and cannot be modified by others. The user who created the script has set the permissions to read and execute only (755), meaning only the owner can edit it.

### How to Run the Script

``` bash 
    ./aws_resource_list.sh <aws_region> <aws_service>
```

Example

```bash
   ./aws_resource_list.sh us-east-1 ec2
```





