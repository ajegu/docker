FROM amazon/aws-cli
ENV DIR=/aws
COPY config /root/.aws/config
COPY credentials /root/.aws/credentials
WORKDIR /aws
ENTRYPOINT [ "aws" ]