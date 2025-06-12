# AWS SAM Hello World Example

This project is a minimal AWS Lambda application built using the [AWS Serverless Application Model (AWS SAM)](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/what-is-sam.html). It uses the **Hello World** starter template and demonstrates the basic setup for deploying a Lambda function using SAM CLI.

---

## 🚀 Features

* Basic AWS Lambda function written in Python
* Exposed via Amazon API Gateway
* Local testing with SAM CLI
* Unit testing with `pytest`

---

## 🛠️ Prerequisites

* [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
* [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html)
* Docker (for local testing and builds)
* Python 3.8 or later

---

## 🧪 Testing Locally

Run the function locally using the provided event:

```bash
sam local invoke HelloWorldFunction --event events/event.json
```

Start the local API Gateway:

```bash
sam local start-api
```

Then visit: `http://localhost:3000/hello`

---

## 🔨 Building the Project

```bash
sam build
```

---

## 📦 Deploying to AWS

To deploy the application to your AWS account:

```bash
sam deploy --guided
```

This will walk you through configuration options including stack name, AWS region, and whether to allow SAM to create roles with required permissions.

---

## ✅ Running Tests

```bash
pytest tests/unit/
```

---

## 📚 Learn More

* [AWS SAM Documentation](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/)
* [SAM CLI GitHub Repo](https://github.com/aws/aws-sam-cli)

---

## 📝 License

This project is licensed under the MIT License.

