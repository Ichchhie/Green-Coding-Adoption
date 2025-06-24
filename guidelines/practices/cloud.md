# Cloud Infrastructure specific suggestions:

1. **Electricity Maps API Usage:** Choose deployment locations based on greener data center availability when possible.

2. **Environment Pruning & Automated Cleanup:**
   - Delete unused or underutilized cloud environments regularly.
   - Perform scheduled shutdowns of environments outside working hours (e.g., 7 PM to 7 AM) or weekends to save energy and cost.
   - Automate daily teardown pipelines to remove test environments after use.
     
4. **Use on-demand computing (serverless computing):**
   - Use technologies like AWS Lambda, which only allocate resources when functions are invoked, rather than keeping processes running continuously. This reduces wasted resources and lowers costs.
5. **Right-Sizing & Resource Allocation by Namespace:**
   - Continuously monitor namespaces or environments to ensure correct CPU/memory allocation.
   - Prevent overprovisioning and balance resource levels with actual needs.
   - Select services based on usage patterns and cost efficiency:
      - Use Lambda for infrequent or short-lived requests.
      - Use EC2 for high-volume or long-running tasks.
   
4. **Batch Scheduling for Energy Efficiency:**
   - Schedule batch jobs during times when energy is greener (e.g., when renewable energy availability is higher).

5. **Auto Scaling Infrastructure:**
   - Automatically scale cloud resources up/down based on real-time demand to reduce waste.
   - Implement scaling down mechanisms to reduce running instances and optimize cost when demand is low.
   - Use infrastructure-as-code (IaC) tools like AWS CDK or Terraform to automate scaling logic (e.g., CPU-based thresholds).
     
7. **Cloud Pricing Tier Optimization:**
Select cloud pricing tiers that fit the deployment environment’s usage profile (e.g., lower tier for non-critical environments).
8. **Use of Infrastructure as Code (IaC):** Deploy and manage infrastructure through code (e.g., AWS CloudFormation, CDK) to enable repeatable, optimized deployments.

