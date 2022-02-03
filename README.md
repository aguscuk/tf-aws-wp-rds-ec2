Original from: https://github.com/aleti-pavan/terraform-aws-wordpress

What's this:
=========

This is to set up wordpress using AWS infrastructure. We are using terraform to provision infrastructure. Code uses and creates following aws services.

1. VPC and it's components
2. Subnets, Route Tables, Internet Gateway, Nat Gateway.
3. EC2 instance
4. EIP for NAT Gateway
5. RDS mysql instance.
6. Security Groups to access both EC2 and MYSQL

Usage:
=======

provisioning:
-------------

1. git clone https://github.com/aguscuk/tf-aws-wp-rds-ec2.git
2. cd tf-aws-wp-rds-ec2
2. terraform init
3. terraform plan
4. terraform apply -auto-approve

Destroying the Infra:
---------------------
1. cd tf-aws-wp-rds-ec2 (Be in the repo directory)
2. terraform destroy -auto-approve

Versions:
--------
Terraform v0.12.24
+ provider.aws v2.12.0
+ provider.template v2.1.2
