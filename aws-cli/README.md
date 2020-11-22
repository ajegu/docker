# AWS CLI

## Build instructions
docker pull amazon/aws-cli

### Build image
docker build -t ajegu/aws .

### Delete image
docker image rm ajegu/aws -f

## Container usage instructions

### Show version
 docker run --rm -it ajegu/aws --version

### Show config
docker run --rm -it ajegu/aws configure list

### Show DynamoDB commands
docker run --rm -it ajegu/aws dynamodb help