☁️ AWS CloudFormation Project — S3 & EC2 Automation
📌 Overview

This project demonstrates the automation of AWS infrastructure using CloudFormation, provisioning both Amazon S3 and Amazon EC2 in a single, reusable template.
It highlights Infrastructure as Code (IaC) principles, allowing reliable, repeatable, and scalable deployment without manual intervention.

🎯 Project Objective

To create robust, reusable CloudFormation templates for automatically deploying AWS resources, ensuring:

✅ Consistency across deployments
✅ Reduced manual setup time
✅ Easy lifecycle management (create, update, delete)

📁 Repository Structure
# Templates
- `templates/temp.yaml` → Simple S3
- `templates/s2+ec2.yaml` → EC2 + S3
- `docs/Presentation1.pdf` → Steps followed

⚙️ Templates Breakdown
🟢 temp.yaml — Simple S3 Template

Deploys a single S3 bucket with a custom name.
Ideal for beginners to understand CloudFormation basics: syntax, parameters, and resource declaration.

🔵 s2+ec2.yaml — EC2 + S3 Combined Template

Deploys EC2 instance + S3 bucket together.

Parameters included:

Instance Type (e.g., t2.micro)
Key Pair Name for SSH access
Bucket Name
Configures security groups and IAM roles (if required).
Demonstrates resource dependency management: ensures EC2 can interact with S3 securely.

🧾 Steps Followed (Reference: Presentation1.pdf)

Designed Templates — Created temp.yaml and s2+ec2.yaml with required resources and parameters.
Validated Templates — Checked for syntax and logical errors in AWS CloudFormation Console.
Created Stacks — Uploaded templates → Entered stack name and parameters → Created stack.
Verified Resources — Confirmed S3 buckets and EC2 instances were deployed successfully.
Tested Functionality — Checked EC2 → S3 connectivity (if applicable).
Deleted Stack — Cleaned up resources automatically to avoid costs.

🛠️ How to Deploy

Via AWS Management Console:

Open CloudFormation → Create Stack → With new resources (standard).
Upload temp.yaml or s2+ec2.yaml.
Fill in parameters: Key Pair, Instance Type, Bucket Name.
Click Create Stack → Wait for CREATE_COMPLETE.
Verify resources in EC2 and S3.
Delete stack when done to remove all resources.

🌟 Key Learnings

Mastered Infrastructure as Code (IaC) concepts.
Gained experience in CloudFormation template structure — Parameters, Resources, Outputs.
Learned stack lifecycle management — creation, update, deletion.
Practiced handling resource dependencies and automation best practices.

🚀 Future Enhancements

Add UserData scripts to EC2 for automatic software deployment.
Attach IAM Role to EC2 for secure S3 access.
Integrate CloudWatch for monitoring and SNS notifications for stack events.
Expand templates for multi-region deployment or multi-AZ setups.

👩‍💻 Author
Anjali Chopariya.
