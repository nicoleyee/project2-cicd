# Project2 deploy-a-high-availability-web-app-using-CloudFormation


## Project Files:
```sh
1- create.sh : Cloudformation create stack script. 
2- update.sh : Cloudformation update stack script.
3- ourinfraServer.yml : Udagram Project's CloudFormation script.
4- ourinfraServerParameters.json : Udagram Project's CloudFormation script parameters.
5- A Diagram for infrastructure and Servers
```
## Instruction of deploy:
Just run;
```sh
> ./create.sh ourinfraServer ourinfraServer.yml ourinfraServerParameters.json
```aws cloudformation create-stack --stack-name udagramApp --template-body file://ourinfraServer.yml --parameters file://ourinfraServerParameters.json --capabilities CAPABILITY_NAMED_IAM
> ./update.sh ourinfraServer ourinfraServer.yml ourinfraServerParameters.json
```aws cloudformation update-stack --stack-name udagramApp --template-body file://ourinfraServer.yml --parameters file://ourinfraServerParameters.json --capabilities CAPABILITY_NAMED_IAM