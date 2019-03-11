# awscloudformation
Test on AWS cloudformation


## App layer
- Key pair credentials need to be pre-created
- `app.yml`

Yaml script to deploy following except DB layer (within 5 mins)
- Create VPC
- Create IG (Internet Gateway)
- Attach IG to VPC
- Create route table for outgoing traffic
- Create private subnets
- Attach routing to private subnets
- Create 2 EC2 instances: instance 1 & 2 on private subnet with Elastic IPs
- Deploy apache on EC2 instances & create simple web app
- Create ACLs for incoming traffic to private subnets
- Create ELB (Elastic Load balancer & targets as instance1 & instance2)
- Create an alias on DNS (route53) to point awscloudformation.org domain to to ELB 
- Setup a monitoring agent for Datadog cloud monitoring

![awscloudformation_setup](https://user-images.githubusercontent.com/41276256/54099108-97d55d00-43f2-11e9-954c-ed68324eeeb0.jpg)
