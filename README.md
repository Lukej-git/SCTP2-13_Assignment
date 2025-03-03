# SCTP2-13_Assignment
# Comparison of Serverless Framework and Terraform for Infrastructure as Code (IaC)

## <u>What type of infrastructure and application deployments are each tool best suited for?</u>

Serverless Framework: Best suited for deploying serverless applications, such as AWS Lambda functions, API Gateway, DynamoDB, and other cloud-managed services. It simplifies serverless application deployment by handling resource provisioning, packaging, and deployment automation.

Terraform: Best suited for provisioning and managing infrastructure across various cloud providers. It is ideal for deploying complete infrastructure stacks, including networks, servers, databases, and security policies.

## <u>How do their primary objectives differ?</u>

Serverless Framework: Focuses on abstracting cloud infrastructure to simplify serverless application deployment and management. It automates the deployment of serverless functions and related resources.

Terraform: Focuses on declarative infrastructure provisioning and management using Infrastructure as Code (IaC). It provides full control over cloud resources, allowing users to define and manage infrastructure components at scale.

## <u>How do they differ in terms of learning curve and ease of use for developers or DevOps teams?</u>

Serverless Framework: Easier for developers who primarily work with serverless applications, as it abstracts many complexities of infrastructure setup. Requires basic YAML configuration and some scripting knowledge.

Terraform: Has a steeper learning curve as it requires understanding HCL (HashiCorp Configuration Language) and the underlying cloud provider services. More suitable for DevOps teams managing complex cloud environments.

## <u>What are the differences in how each tool handles state tracking and deployment changes?</u>

Serverless Framework: Uses AWS CloudFormation or its own deployment tracking to manage state. Deployment changes are managed automatically with rollback capabilities.

Terraform: Uses a state file (stored locally or remotely) to track the current state of deployed infrastructure. It provides an execution plan (terraform plan) before applying changes to ensure predictability.

## <u>In what scenarios would you recommend using Serverless Framework over Terraform, and vice versa?</u>

### Use Serverless Framework when:

- Deploying serverless applications with AWS Lambda, API Gateway, and DynamoDB.

- Developers want a quick and simple way to deploy serverless functions.

- Managing event-driven applications or microservices architectures.

### Use Terraform when:

- Managing full cloud infrastructure, including networks, virtual machines, databases, and security policies.

- Deploying multi-cloud or hybrid cloud environments.

- Needing infrastructure versioning, state management, and advanced automation.

## <u>Are there scenarios where using both together might be beneficial?</u>

Yes, using both tools together can be beneficial in the following scenarios,

- Hybrid Approach: Use Terraform to provision the foundational infrastructure (VPCs, databases, security groups) while using Serverless Framework to deploy and manage serverless applications.

- Separation of Concerns: DevOps teams can use Terraform for infrastructure provisioning, while developers use Serverless Framework to deploy and manage application logic.

- Multi-cloud Environments: Terraform can manage infrastructure across different cloud providers, while Serverless Framework handles function deployment for AWS serverless services.
