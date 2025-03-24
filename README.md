# NetworkSecurity_NDR_NetworkSensor
This repo is intended to help you deploy your own Trend Vision One Network Sensor (NDR)

aws cloudformation create-stack --stack-name V1NetSec --template-body file://TrendNDR_Instance.yml --parameters ParameterKey=Token,ParameterValue="$TOKEN_CONTENT"


``
aws cloudformation create-stack --stack-name V1NetSec \
--template-body file://TrendNDR_Instance.yml \
--parameters \
ParameterKey=Token,ParameterValue="$TOKEN_CONTENT" \
ParameterKey=VPC,ParameterValue="$VPC_ID" \
ParameterKey=DataSubnet,ParameterValue="$DATA_SUBNET_ID" \
ParameterKey=ManagementSubnet,ParameterValue="$MANAGEMENT_SUBNET_ID" \
ParameterKey=KeyName,ParameterValue="$KEY_NAME" \
ParameterKey=InstanceType,ParameterValue="$INSTANCE_TYPE" \
ParameterKey=ImageId,ParameterValue="$IMAGE_ID" \
ParameterKey=InstanceName,ParameterValue="$INSTANCE_NAME"
``
