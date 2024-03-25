

## Serverless-Web-Application

### Overview:

This project showcases a serverless web application allowing users to request unicorn rides from the Wild Rydes fleet. It's important to note that this is a fictional service designed primarily to illustrate serverless architecture principles. The application provides an HTML-based user interface for users to indicate their pickup location and interacts with a RESTful web service on the backend to submit ride requests and dispatch nearby unicorns. Additionally, users can register and log in before requesting rides.

### Application Architecture:

The application architecture relies on several AWS services including Lambda, API Gateway, DynamoDB, Cognito, and Amplify Console. Amplify Console facilitates continuous deployment and hosting of static web resources like HTML, CSS, JavaScript, and images. JavaScript executed in the browser communicates with a public backend API built using Lambda and API Gateway. Cognito manages user authentication to secure the backend API, while DynamoDB provides a persistence layer for data storage. Furthermore, Amazon Route 53 can be utilized for domain name setup.

![Serverless Application Architecture](https://github.com/DimitryZH/Serverless-Web-Application/assets/146372946/0abaeea5-040f-48d9-a90d-49b7f853ce99)

### Implementation:

To explore the deployed application, visit [this link](https://wildrydes.dmitry-web.com/).
- **Note: In my case, I used my own `dmitry-web.com` domain name for the deployment.**
#### Steps:

1. **Setting Up AWS Accounts:**

    - **Access AWS Management Console:**
      - Log in to the AWS Management Console.
      
    - **Configure IAM Users and Roles:**
      - Navigate to IAM in the console.
      - Click on "Users" and then "Add user."
      - Attach necessary policies to grant permissions for accessing AWS services.
      - Create user details and generate Access Key ID and Secret Access Key.
      
    - **Generate Access Keys:**
      - Access user details in the IAM dashboard.
      - Under "Security credentials," click "Create access key."
      - Download the credentials file or copy Access Key ID and Secret Access Key.
      
2. **Building the Wild Rydes Application:**

    - **Create Lambda Functions:**
      - Define the business logic for the application.
      - Navigate to Lambda service in the console.
      - Create functions, upload code, and configure settings.
      - Test functions to ensure functionality.
      
    - **Set Up API Gateway Endpoints:**
      - Define API endpoints for user interaction.
      - Navigate to API Gateway service in the console.
      - Create API, resources, methods, and integrations with Lambda functions.
      - Deploy the API to make it accessible.
      
    - **Integrate with DynamoDB for Data Storage:**
      - Design data model for application data.
      - Access DynamoDB service in the console.
      - Create tables, define schema, and configure permissions.
      - Implement logic in Lambda functions to interact with DynamoDB.
      
3. **Deploying and Testing the Application:**

    - **Package and Deploy Lambda Functions:**
      - Package function code and dependencies.
      - Deploy functions in the Lambda console.
      
    - **Deploy API Gateway Configuration:**
      - Deploy the API in the API Gateway console.
      
    - **Test API Endpoints:**
      - Send requests to API endpoints.
      - Verify responses and functionality.
      
    - **Invoke Lambda Functions:**
      - Test integration between API Gateway and Lambda functions.
      - Monitor execution in the Lambda console.
      
    - **Verify Data Storage in DynamoDB:**
      - Access DynamoDB tables in the console.
      - Perform CRUD operations to ensure data integrity.

For a comprehensive guide, you can follow detailed instructions [here](https://aws.amazon.com/getting-started/hands-on/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito/?ref=gsrchandson) provided by AWS. These steps enable setting up AWS accounts, building the Wild Rydes application, deploying it to AWS, and testing its functionality, offering hands-on experience with serverless architecture and AWS services.
