# Infrastructure-as-Code-for-Thought-Machine

This repository consists of a YAML template intended for the automated provisioning and configuration of Thought Machine's Vault service into AWS. This template deploys a VPC, with a pair of public and private subnets spread across two Availability Zones. It deploys an internet gateway, with a default route on the public subnets. It deploys a pair of NAT gateways (one in each AZ), and default routes for them in the private subnets. Additionally, it deploys EKS control plane and worker node resources to run the microservices that make up Vault. Lastly, it deploys a PostgreSQL RDS instance as the data store. A diagram illustrating this can be seen below:

![image](https://github.com/ali-alwan99/Infrastructure-as-Code-for-Thought-Machine/assets/128723860/f9585c92-2a94-4822-bcbc-98f49205a25a)
