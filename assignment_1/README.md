We need to run the below steps to create infrastructure.

* terraform init is to initialize the working directory and downloading plugins of the provider.
* terraform plan is to create the execution plan for our code.
* terraform apply is to create the actual infrastructure. It will ask you to provide the Access Key and Secret Key in order to create the infrastructure. So, instead of hardcoding the Access Key and Secret Key, it is better to apply at the run time.

**Next Step:- Verify the resources**

* Terraform will create below resources

    *  VPC
    *  Application Load Balancer
    *  Public & Private Subnets
    *  EC2 instances
    *  RDS instance
    *  Route Table
    *  Internet Gateway
    *  Security Groups for Web & RDS instances
    *  Route Table

Once the resource creation finishes you can get the DNS of a load balancer and paste it into the browser and you can see load balancer will send the request to two instances.

That’s it now, this is how we can create three-tier architecture in AWS using Terraform.
