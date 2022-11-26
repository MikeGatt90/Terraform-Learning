For a free diagramming tool you can use [https://app.diagrams.net/](https://app.diagrams.net/ "‌") (there are others out there, but stick with free).

How to diagram an AWS Architecture with [Draw.io](http://Draw.io "‌"): [https://youtu.be/tSqEljKKiU0](https://youtu.be/tSqEljKKiU0 "‌")

NOTE: Use the Terraform documentation to build out your code. You should not be copying and pasting a past or current guest’s code.

Your team needs you to diagram and deploy a two-tier architecture for your company. For the Foundational project you are allowed to have all your code in a single [main.tf](http://main.tf "‌") file (known as a monolith) with hardcoded data.

1. Deploy a VPC with CIDR 10.0.0.0/16 with 2 public subnets with CIDR 10.0.1.0/24 and 10.0.2.0/24. Each public subnet should be in a different AZ for high availability.
2. Create 2 private subnet with CIDR ‘10.0.3.0/24' and '10.0.4.0/24' with an RDS MySQL instance (micro) in one of the subnets. Each private subnet should be in a different AZ. Note that you don’t want the size of your RDS to big too big or it will take an extra long time to deploy.
3. A load balancer that will direct traffic to the public subnets.
4. Deploy 1 EC2 t2.micro instance in each public subnet.

