# NetworkSecurity_NDR_NetworkSensor
This repo is intended to help you deploy your own Trend Vision One Network Sensor (NDR)

aws cloudformation create-stack --stack-name V1NetSec --template-body file://ec2-instance.yml --parameters ParameterKey=Token,ParameterValue="$TOKEN_CONTENT"
