# Serverless Movies API

### Project Overview:

- Create a rest API which give a list of movies. We will use some AWS Services, AWS SAM CLI, S3, Lambda, DynamoDB and APIGateway. Build the project using only SDK, i.e. Visual Studio + CLI (try do not use the AWS console).

### Prerequisites:

- AWS account
- Docker account (just running in the background)
- I will use Javascript for Lambdas functions (DO NOT USE TYPESCRIPT, it will save a lot of headaches) but you can use any language.

### Setup Instructions:

- Initialize AWS SAM, "sam init" (Quick Start Templates, node+zip for me because I'm using JavaScript). Choose Hello World Example.
- Install dependencies, node (npm init -y), AWS SDK (npm install aws-sdk).
- Configure AWS credentials, preferentially use SSO Login (check by bash project for more details).
- Create "src", "src/handlers/getMovies.js", "src/models/movies.js".

### Building the Project:

- Copy the code for getMovies.js
- Copy template.yaml

### Deploying the Project:

- Build your app with "sam build".
- Deploy with "sam deploy --template-file
  template.yaml --stack-name THE-NAME-U-WANT --resolve-s3 --capabilities CAPABILITY_IAM".

### Testing the API:

- After deployment, you'll receive the API Gateway URL. You can test your endpoints using tools like curl, Postman, or directly from the browser.
