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

---

# AWS deployment (optional)

### Create an AWS Account
<details>
    <summary>Click for Step-by-Step tutorial</summary>
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

### Create an AWS Elastic Beanstalk Service [Back]
<details>
    <summary>Click for Step-by-Step tutorial</summary>
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

### Create an AWS IAM User without Console Access
<details>
    <summary>Click for Step-by-Step tutorial</summary>
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

### Link a GitHub Repo with CircleCI
<details>
    <summary>Click for Step-by-Step tutorial</summary>
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

4. **Navigate to Environment Variables:**
   - In the project settings, navigate to the "Environment Variables" or "Environment" section.

5. **Add New Environment Variables:**
   - Click on the "Add Environment Variable" button to add a new environment variable.

6. **Enter Variable Name and Value:**
   - Enter "AWS_ACCESS_KEY_ID" as the variable name and provide the corresponding AWS access key ID in the value field.

7. **Repeat for AWS_SECRET_ACCESS_KEY:**
   - Similarly, add another environment variable named "AWS_SECRET_ACCESS_KEY" and provide the corresponding AWS secret access key as the value.

8. **Save Environment Variables:**
   - Save the environment variables to ensure that they are securely stored and accessible during the build and deployment processes.

9. **Verify Configuration:**
   - Verify the environment variable configuration by triggering a new build in CircleCI that utilizes the AWS credentials. Ensure that the build process executes without any issues related to AWS authentication.

</details>

### Create an AWS S3 Bucket and Making It Publicly Accessible [Front]
<details>
    <summary>Click for Step-by-Step tutorial</summary>
1. **Sign In to AWS Management Console:**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in to your AWS account with appropriate administrative privileges.

2. **Navigate to S3:**
   - In the AWS Management Console, navigate to the Amazon S3 (Simple Storage Service) service.

3. **Click on "Create Bucket":**
   - Click on the "Create Bucket" button to begin creating a new S3 bucket.

4. **Provide Bucket Details:**
   - Enter a unique and descriptive name for your S3 bucket, select the region where you want the bucket to be stored, and configure any additional settings as needed.

5. **Configure Public Access Settings:**
   - In the "Set permissions" section, ensure that the bucket and its objects are publicly accessible by unchecking the "Block all public access" option. Be aware of the implications of making the bucket publicly accessible and ensure that you have taken necessary security measures to protect sensitive data.

6. **Configure Bucket Properties:**
   - Configure the properties of the bucket, including versioning, logging, and other settings based on your specific requirements.

7. **Review and Create the Bucket:**
   - Review all the settings to ensure they align with your intended configuration. Click on the "Create bucket" button to create the S3 bucket.

8. **Upload Objects and Set Public Access:**
   - Upload the desired objects to the S3 bucket. Select the uploaded objects and configure their permissions to be publicly accessible. You can set the object's access control list (ACL) to "public" or configure a bucket policy to make all objects public.

9. **Verify Public Access:**
   - Verify the public accessibility of the S3 bucket and its objects by testing the access URL in a web browser or via the AWS CLI.
</details>

### Create an AWS PostgreSQL Publicly Accessible Database [DB]
<details>
    <summary>Click for Step-by-Step tutorial</summary>
1. **Sign In to AWS Management Console:**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in to your AWS account with appropriate administrative privileges.

2. **Navigate to RDS:**
   - In the AWS Management Console, navigate to the Amazon RDS (Relational Database Service) service.

3. **Click on "Create Database":**
   - Click on the "Create database" button to begin the process of creating a new PostgreSQL database.

4. **Select PostgreSQL Engine:**
   - Choose the PostgreSQL engine as the database creation option.

5. **Choose Use Case:**
   - Select the appropriate use case option for your PostgreSQL database, such as production, development, or testing.

6. **Configure Database Settings:**
   - Configure the necessary settings for your PostgreSQL database, including database instance specifications, storage, and connectivity settings.

7. **Set Access Permissions:**
   - Define the security and access settings for your database, including the creation of a master username and password. Ensure that the database is publicly accessible by configuring the security group settings to allow inbound traffic from your desired IP addresses or specifying a public IP range (0.0.0.0/0).

8. **Configure Additional Settings (Optional):**
   - Optionally, configure additional settings for the database, such as backup and maintenance options, monitoring, and performance insights.

9. **Review and Create the Database:**
   - Review all the configuration details to ensure they align with your intended database setup. Click on the "Create database" button to create the PostgreSQL database.

10. **Verify Database Connectivity:**
    - Verify the connectivity to the PostgreSQL database by using appropriate client tools or by connecting to the database instance from your application. Ensure that the necessary security measures are in place to protect sensitive data and prevent unauthorized access.
</details>

### Add the enviroument varables to ElasticBeanstalk config

* DB_NAME
* DB_USER
* DB_PASSWORD
* DB_HOST
* DB_PORT

<details>
    <summary>Click for Step-by-Step tutorial</summary>
1. **Sign In to AWS Management Console:**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in to your AWS account with appropriate administrative privileges.

2. **Navigate to Elastic Beanstalk:**
   - In the AWS Management Console, navigate to the Amazon Elastic Beanstalk service.

3. **Select Your Application:**
   - Choose the application that corresponds to the Elastic Beanstalk environment where you want to set the environment variables.

4. **Select the Environment:**
   - Select the specific environment within the application where you wish to configure the environment variables.

5. **Navigate to Configuration:**
   - In the selected environment's dashboard, navigate to the "Configuration" section.

6. **Click on Software Configuration:**
   - Click on the "Edit" button in the "Software" configuration category to edit the software configuration of the environment.

7. **Set Environment Variables:**
   - Under the "Environment properties" or "Environment variables" section, add the desired environment variables by providing the variable names and corresponding values.

8. **Save Configuration Changes:**
   - After adding the environment variables, save the configuration changes to apply the new environment variables to the Elastic Beanstalk environment.

9. **Verify Environment Variable Configuration:**
   - Verify that the environment variables are correctly set and accessible within the Elastic Beanstalk environment. You can check the environment variables' values by logging into the environment or by accessing them programmatically from within your application.
</details>