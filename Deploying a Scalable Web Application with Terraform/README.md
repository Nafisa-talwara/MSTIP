# Deploying-a-Scalable-Web-Application-on-AWS-with-Terraform
# Overview
This project leverages the power of AWS to create a robust and scalable web application. By using Terraform, we can manage our infrastructure as code, making it easy to deploy and manage resources consistently. The application is designed to handle variable loads, thanks to the Auto Scaling feature and the Application Load Balancer.
# Architecture
 * Amazon EC2: Virtual servers that host the web application.
 * Application Load Balancer (ALB): Distributes incoming traffic across multiple EC2 instances to ensure high availability.
 * Auto Scaling: Automatically adjusts the number of EC2 instances based on demand.
# Getting Started
1. So, let’s start by configuring AWS credentials first. Also, make sure the latest version of Terraform is installed on your system.
2. To configure AWS credentials in Visual Studio Code (VS Code), you can use the AWS Command Line Interface (CLI) command: aws configure.
3. Enter Your Credentials like:
   * AWS Access Key ID
   * AWS Secret Access Key
   * Default region name: us-east-1.
4. "aws configure list", this command will create a configuration file at ~/.aws/config and a credentials file at ~/.aws/credentials, storing your AWS credentials securely.
   
    ![WhatsApp Image 2025-06-17 at 18 32 02_d1277a61](https://github.com/user-attachments/assets/8144743d-2796-42fd-89ab-9c4f3bf0ff1c)

6. Move on to running the Terraform init, plan, and apply commands to see whether the above code files are working or not.

   ![image](https://github.com/user-attachments/assets/9e94d6eb-aed4-4382-879d-29fe49ff120d)
   
   * Terraform Apply:
     
   ![image](https://github.com/user-attachments/assets/180c95be-8d92-4ec6-8d3e-879559cf0681)
7. log in to your AWS account to check whether the resources have been created. Specifically, verify the ELB to ensure it is healthy. Only then will you be able to access the URL.
# Conclusion:
By using Terraform, we successfully automated the provisioning of a scalable AWS infrastructure, including networking components, security groups, and EC2 instances behind an Application Load Balancer. This approach not only simplifies deployment but also ensures consistency and repeatability across environments. With Terraform, managing cloud resources becomes efficient, reducing manual effort and the risk of configuration errors. You can now extend this setup by integrating monitoring, auto-scaling, or containerized applications for even greater flexibility.
