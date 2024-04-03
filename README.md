# aws lambda in bash

for plain bash it's super simple
```
sam build
sam deploy --guided
```

For aws-cli this means creating an ECR repo with an image that has the AWS CLI in it.

I created pull-through cache in ECR (manually) and pulling an image into it:

```
docker pull 1234567890.dkr.ecr.us-east-1.amazonaws.com/ecr-public/aws-cli/aws-cli:2.15.34
```
