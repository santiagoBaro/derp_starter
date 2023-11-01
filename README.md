# derp_starter
## Welcome to our Starter Project!

This project is designed to serve as a convenient starting point for your development journey. You can fork this repository and kickstart your coding process right away. It is tailored to provide a seamless integration of Django, React, and PostgreSQL, offering a robust and versatile development stack.

With a Dockerized setup, local development becomes hassle-free, allowing you to focus on building your application without worrying about complex environment setup. The Docker containers streamline the process, ensuring consistency and simplicity throughout the development cycle.

Moreover, we have implemented a CircleCI workflow specifically tailored for AWS deployment. This integration simplifies the deployment process, enabling you to effortlessly deploy your application to an AWS environment. The CircleCI pipeline has been optimized to handle the deployment workflow efficiently, granting you the freedom to concentrate on refining your application's features and functionalities.

We hope this project serves as a valuable tool to expedite your development process, empowering you to concentrate on creating an exceptional application experience. Happy coding!

## Prerequisites for the Project

- Docker: Containerization platform for packaging, deploying, and running applications.
- Node.js: JavaScript runtime for building scalable and efficient applications.

## Installing Prerequisites

### Docker Installation

If Docker is not already installed, follow the steps below:

1. **For Linux**:
   - Run the following command in the terminal:
     ```bash
     sudo apt-get update
     sudo apt-get install docker-ce docker-ce-cli containerd.io
     ```

2. **For macOS** and **Windows**:
   - Download the Docker Desktop installer from the official [Docker website](https://www.docker.com/products/docker-desktop) and follow the installation instructions.

### Node.js Installation

If Node.js is not already installed, follow the steps below:

1. **For Linux**:
   - Run the following commands in the terminal:
     ```bash
     sudo apt-get update
     sudo apt-get install nodejs
     sudo apt-get install npm
     ```

2. **For macOS** and **Windows**:
   - Download the Node.js installer from the official [Node.js website](https://nodejs.org/en/download/) and follow the installation instructions.

After installing Docker and Node.js, ensure that the versions are compatible with the project requirements.

======

# AWS deployment (optional)
## Step-by-Step Guide to Link a GitHub Repo with CircleCI
<details>
    <summary>Click to expand!</summary>
## Step-by-Step Guide to Link a GitHub Repo with CircleCI

1. **Sign in to CircleCI:**
   - Visit the [CircleCI website](https://circleci.com) and sign in using your GitHub account.

2. **Set Up a New Project:**
   - Once signed in, click on the "Add Projects" or the "+" icon in the sidebar.
   - Select the organization and the GitHub repository you want to link with CircleCI.

3. **Configure Your Project:**
   - Find the repo and select `Set Up Project`
   - Choose the first option `Fastest`
   - Choose `main` as the brach
   - CircleCI will detect your project's configuration file automatically, typically named `.circleci/config.yml`.
</details>

## Step-by-Step Guide to Creating an AWS Account
<details>
    <summary>Click to expand!</summary>
1. **Visit the AWS Website:**
   - Go to the [AWS website](https://aws.amazon.com/).

2. **Click on "Create an AWS Account":**
   - Click on the "Create an AWS Account" button.

3. **Sign In or Create a New Account:**
   - Sign in using your existing Amazon account or create a new one.

4. **Provide Account Information:**
   - Enter your email address, password, and an AWS account name.

5. **Contact Information:**
   - Enter your name, address, and phone number.

6. **Payment Information:**
   - Enter your payment information. AWS requires a valid credit card for account verification purposes. However, you can use the AWS Free Tier to explore services for a limited time without any charges.

7. **Phone Verification:**
   - AWS may require phone verification to ensure the security of your account. Enter the code sent to your phone to verify your identity.

8. **Select a Support Plan (Optional):**
   - Choose a support plan that aligns with your requirements. AWS offers various support plans with different levels of service and features.

9. **Read and Accept AWS Customer Agreement:**
   - Carefully read the AWS Customer Agreement, and if you agree with the terms, click on the "Create Account and Continue" button.

10. **Confirmation:**
    - Once your account is successfully created, AWS will provide you with a confirmation message. You can now sign in to your AWS Management Console.

11. **Configure Security Settings:**
    - Follow the AWS security best practices and configure security settings, such as setting up multi-factor authentication (MFA) and creating strong IAM policies.
</details>

## Step-by-Step Guide to Creating an AWS Elastic Beanstalk Service
<details>
    <summary>Click to expand!</summary>
1. **Sign In to AWS Management Console:**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in to your AWS account.

2. **Navigate to Elastic Beanstalk:**
   - In the AWS Management Console, navigate to the Elastic Beanstalk service.

3. **Click on "Create New Application":**
   - Click on the "Create New Application" button to begin the process of creating a new application environment.

4. **Select Application Platform:**
   - Choose the application platform that best suits your requirements, such as Python, Java, Node.js, PHP, Ruby, Docker, or Go.

5. **Choose Application Code:**
   - Select the application code source, either from the AWS CodeCommit repository, AWS CodePipeline, GitHub, or your own source.

6. **Configure Application Details:**
   - Enter the necessary details for your application, such as the application name, platform version, and other configuration settings.

7. **Configure Environment:**
   - Configure the environment type (Web server environment or Worker environment), instance type, environment name, and other environment-specific settings.

8. **Configure Additional Options:**
   - Set up additional options, such as load balancer configuration, database settings, environment variables, and other advanced configurations if required.

9. **Review Configuration Details:**
   - Review all the configuration details to ensure they are accurate and meet your application requirements.

10. **Create the Application:**
    - Click on the "Create Application" button to create your AWS Elastic Beanstalk application. AWS will start the process of provisioning the necessary resources and deploying your application.

11. **Monitor Application Deployment:**
    - Monitor the deployment process through the AWS Management Console or AWS Elastic Beanstalk console to ensure that your application is deployed successfully.

12. **Test and Verify the Application:**
    - Test your application to verify that it is functioning correctly in the AWS Elastic Beanstalk environment.
</details>

## Step-by-Step Guide to Creating an AWS IAM User without Console Access
<details>
    <summary>Click to expand!</summary>
1. **Sign In to AWS Management Console:**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in to your AWS account with appropriate administrative privileges.

2. **Navigate to IAM:**
   - In the AWS Management Console, navigate to the IAM (Identity and Access Management) service.

3. **Access the Users Section:**
   - From the IAM dashboard, click on the "Users" tab located in the left-hand navigation pane.

4. **Click on "Add User":**
   - Click on the "Add User" button to begin creating a new IAM user.

5. **Provide User Details:**
   - Enter the desired username for the new IAM user and select the "Programmatic access" option to grant access via the AWS API, CLI, SDKs, or other development tools.

6. **Set Permissions:**
   - Configure the necessary permissions for the IAM user by attaching appropriate policies that define the user's access to AWS services and resources. Ensure that the policies are restricted and aligned with the principle of least privilege.

7. **Configure Tags (Optional):**
   - Optionally, you can configure tags to help categorize and manage your IAM users effectively.

8. **Review User Details:**
   - Review the user details, including the username, access type, and assigned permissions, to ensure they align with the intended access requirements.

9. **Create the IAM User:**
   - Click on the "Create User" button to create the IAM user. AWS will generate an access key ID and secret access key for the user.

10. **Store Access Keys Securely:**
    - It is crucial to securely store the access key ID and secret access key as they provide programmatic access to your AWS resources. Consider using AWS Secrets Manager or another secure storage solution to manage the access keys.
</details>