# Synapxe-Assignment
Synapxe-Assignment for Cloud Engineer

## PropertyGuru Infrastructure on AWS with Terraform (Assignment)

This assignment evaluates your understanding of Infrastructure as Code (IaC) principles and your ability to deploy a scalable, secure, and cost-effective infrastructure for PropertyGuru, a property website, on AWS in the Singapore region.

**Scenario:**

- PropertyGuru anticipates 100,000 users per month.
- The application is a 3-tier LAMP stack (Linux, Apache, MySQL, PHP).
- Expect high volumes of user-uploaded files, images, and videos.
- The annual budget is approximately $1 million USD.
- The development team embraces IaC using Terraform.

**Objectives:**

- **Design** and implement a secure, reliable, and scalable infrastructure on AWS using Terraform.
- Demonstrate cost-effectiveness within the provided budget constraints.
-  **Optionally** (bonus points): Include a basic CI/CD pipeline for automated infrastructure provisioning.
- Provide clear documentation for your solution.

**Tasks:**

1. **Infrastructure Design (Documentation):**
   - Create a high-level architecture diagram (optional) showcasing the components of your infrastructure (VPC, Subnets, Security Groups, etc.).
   - Document the specific AWS services you plan to utilize and their roles within the architecture.
   - Explain the rationale behind your design choices, considering security, scalability, and performance.

2. **Terraform Configuration:**
   - Implement Terraform code in `main.tf` or modular files (`modules/`) to define the infrastructure resources.
   - Configure variables (in `variables.tf` or `terraform.tfvars`) for flexibility and environment-specific adjustments.
   - Ensure code adheres to best practices for readability, maintainability, and security.
   - Consider using appropriate AWS resources for:
     - VPC with public and private subnets (consider availability zones for resiliency)
     - Internet Gateway (public subnet access)
     - Route tables and associations
     - Security Groups for web servers, database, and load balancer (initially allow basic access, adjust later)
     - (Optional) Elastic Block Store (EBS) volumes for persistent storage
     - (Optional) Auto Scaling groups for web servers for horizontal scaling
     - **Important:** Remember to review and adjust security group rules as needed.

3. **CI/CD Pipeline (Optional):**
   - (Bonus points) Implement a basic CI/CD pipeline using tools like Terraform Cloud, AWS CodeBuild, or your preferred solution.
   - This pipeline should automate Terraform code validation, testing (if possible), and infrastructure provisioning on AWS. 

4. **Documentation:**
   - Provide clear and concise documentation within the README.md file explaining the infrastructure design, Terraform code structure, and deployment steps (including any commands and dependencies).
   - Include instructions for using and customizing the Terraform configuration.

**Evaluation Criteria:**

- Completeness and correctness of infrastructure design (architecture diagram and documentation).
- Efficiency and cost-effectiveness of the chosen AWS services.
- Comprehensiveness and organization of Terraform code.
- (Optional) Functionality and implementation of the CI/CD pipeline.
- Clarity and conciseness of documentation (README.md).

**Deliverables:**

- A GitHub repository containing all Terraform code, documentation (README.md), and optional CI/CD pipeline scripts.
- A well-structured presentation explaining your design decisions and showcasing the infrastructure configuration.

**Hints:**

- Consider leveraging Terraform modules for reusability and modularity of your code.
- Explore AWS services that optimize performance and cost-efficiency for high-traffic web applications.
- Review security best practices and implement appropriate access controls for your resources.
- Document assumptions and trade-offs made in your design.

This assignment allows you to showcase your expertise in IaC and your ability to design a scalable and cost-effective infrastructure solution for PropertyGuru.

