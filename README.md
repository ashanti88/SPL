# SPL

This Cloudformation template creates following resourses: 
1. EC2 Instance 
2. Application Load Balancer + Listener 
3. Autoscaling Group  - to provide extra instances in case of high traffic utilization. 
4. EC2 Target Group 
5. Launch configuration for autoscaling group. 
6. 2 Security Groups for EC2 Instance and ELB

EC2 instance using userdata to install Apache2 server, start it and output result of the exit status. 
Template provides parameters for users to specify networking bits.
