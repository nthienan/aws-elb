# CloudFormation Templates for Getting Started Tutorial with AWS Elactis Load Balacing
- ### Classic load balancer: 
  
  - **Create stack**:
    ```bash
    aws cloudformation create-stack --stack-name clb-getting-started --template-body file://classic-elb.yaml --parameters ParameterKey=KeyName,ParameterValue=<existing-ec2-key-pair-name>
    ```

  - **Update stack**:
    ```bash
    aws cloudformation update-stack --stack-name clb-getting-started --template-body file://classic-elb.yaml --parameters ParameterKey=KeyName,ParameterValue=<existing-ec2-key-pair-name>
    ```

  - **Delete stack**:
    ```bash
    aws cloudformation delete-stack --stack-name clb-getting-started
    ```

  - **Describe stack**:
    ```bash
    aws cloudformation describe-stacks --stack-name --stack-name clb-getting-started
    ```