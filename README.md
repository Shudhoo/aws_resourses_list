AWS Resource Monitoring Script
About
Hi everyone! This project showcases my learning in Linux OS and fundamentals of Linux, with a focus on shell scripting, which is crucial for DevOps and Cloud Engineers in daily tasks.

This script helps you list AWS services running on your account, such as EC2, S3, RDS, Lambda, etc. It saves time by eliminating the need to manually check resources and compile reports. Instead of running multiple AWS CLI commands, this script provides all the necessary information in one go.

Prerequisites
Before running this script, ensure the following are set up:

1️⃣ Install AWS CLI
Run the following commands to install AWS CLI:

bash
Copy
Edit
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
2️⃣ Configure AWS CLI
Set up AWS CLI with your credentials using:

bash
Copy
Edit
aws configure
🔹 For reference, visit the AWS CLI documentation.

How to Run the Script
Simply execute the script using:

bash
Copy
Edit
./aws_resource_list.sh <aws_region> <aws_service>
🔹 Example:

bash
Copy
Edit
./aws_resource_list.sh us-east-1 ec2
Permissions
This script is assigned 775 permissions, meaning:

Owner can read, write, and execute

Group & Others can read and execute, but cannot modify

Only the creator can edit the script.

Contributions & Support
Feel free to use this script, but modifications require proper permissions.

If you find issues or improvements, feel free to suggest them.
