# Welcome to this CDK TypeScript project

This project demonstrates how to create a simple "Hello World" AWS Lambda function using Golang and deploy it using AWS CDK in Typescript. The Lambda function is invoked via an API Gateway endpoint.

## Prerequisites

- Nodejs
- AWS CDK
- Go

## Setup

1. Clone the repository: 
    ```sh
    git clone git@github.com:milavernazza/modak.git
    cd modak
    ´´´
2. Install the CDK dependencies: 
    ```sh
    cd cdk-hello-world
    npm install
    ´´´    
3. Build the Golang application: 
    ```sh
    cd ../hello-world
    GOOS=linux GOARCH=amd64 go build -0 main main.go
    ´´´

3. Deploy the CDK stack: 
    ```sh
    cd ../cdk-hello-world
    cdk deploy
    ´´´
## GitHub Actions

The project is set up with GitHub Actions to automate the deployment process.
Any push to the 'main' branch will trigger the deployment workflow.

## License

This project is licensed under the MIT License.