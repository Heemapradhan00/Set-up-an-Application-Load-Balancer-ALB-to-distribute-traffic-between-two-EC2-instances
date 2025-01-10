# Set-up-an-Application-Load-Balancer-ALB-to-distribute-traffic-between-two-EC2-instances
Here is the final README file for your simple load balancer setup:

## Objective:
This task involves setting up an Application Load Balancer (ALB) to evenly distribute incoming traffic across two EC2 instances.

## Steps:

1. **Launch EC2 Instances:**
   - Create two EC2 instances in the same region.
   - Install a web server (e.g., Apache or Nginx) on each instance.
   - Configure each instance with a unique HTML page to identify traffic distribution.

2. **Create the Load Balancer:**
   - Go to the AWS Management Console and navigate to **EC2 > Load Balancers**.
   - Select **Application Load Balancer** and configure it:
     - Specify the VPC and subnets.
     - Add the two EC2 instances as targets in the target group.

3. **Test the Setup:**
   - Retrieve the DNS name of the load balancer from the console.
   - Open the DNS in a browser and refresh multiple times to see traffic alternating between the two EC2 instances.

## Notes:
- Ensure the EC2 instances are in a security group that allows HTTP traffic (port 80).
- Use IAM roles for secure access if needed.
- Monitor the health and performance of instances through CloudWatch metrics.

