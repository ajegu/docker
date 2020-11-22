# AWS CLI

## Build instructions
docker pull amazon/aws-cli

## Container usage instructions

### Show version
 docker run --rm -it amazon/aws-cli --version

### Show config
docker run --rm -it -v ~/.aws:/root/.aws amazon/aws-cli configure list

### Show DynamoDB commands
docker run --rm -it -v ~/.aws:/root/.aws amazon/aws-cli dynamodb help