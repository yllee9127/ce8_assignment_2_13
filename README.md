# ce8_assignment_2_13

Assignment 2.13

Make a comparison between Serverless Framework and Terraform as tools for IaC. answer the following:

Question 1 - What type of infrastructure and application deployments are each tool best suited for?

Answer - The Serverless Framework is designed specifically for building and deploying serverless applications. It abstracts much of the complexity associated with managing serverless architectures, such as AWS Lambda, Google Cloud Functions, and Azure Functions. Developers can focus more on writing business logic rather than managing infrastructure.
Terraform, on the other hand, is a general-purpose infrastructure as code (IaC) tool that supports a wide range of cloud services. While it can certainly manage serverless resources, it doesn’t offer the same level of abstraction and ease of use for serverless-specific tasks as the Serverless Framework.

Reference: The Advantages of Using Serverless Framework Over Terraform | by Dorian Machado | Medium (https://dorian599.medium.com/the-advantages-of-using-serverless-framework-over-terraform-136f358454bf)


Question 2 - How do their primary objectives differ?

Answer - Terraform mainly handles infrastructure provisioning across multiple clouds and SaaS providers and manages the entire lifecycle of the infrastructure. 
Serverless Framework provides an excellent set of tools to manage the deployment and management of serverless applications. It offers a streamlined workflow and a great developer experience, with support for multiple serverless providers.  

Reference: Terraform vs Serverless Framework - Glen Thomas (https://blog.glen-thomas.com/aws/platform-engineering/terraform/serverless/iac/2022/08/18/terraform-vs-serverless.html)


Question 3 - How do they differ in terms of learning curve and ease of use for developers or DevOps teams?

Answer - Terraform has a steeper learning curve than the Serverless Framework. Terraform’s configuration language can be more complex and requires a deeper understanding of infrastructure concepts. The Serverless Framework, on the other hand, is more straightforward and easier to learn for developers who are new to serverless architecture.

Reference: Terraform vs Serverless Framework - Glen Thomas (https://blog.glen-thomas.com/aws/platform-engineering/terraform/serverless/iac/2022/08/18/terraform-vs-serverless.html)


Question 4 - What are the differences in how each tool handles state tracking and deployment changes?

Answer - Terraform’s state management system enables you to keep track of the current state of your infrastructure and make changes accordingly. The Serverless Framework does not have a state management system, which can make it harder to manage complex applications.

Reference: Terraform vs Serverless Framework - Glen Thomas (https://blog.glen-thomas.com/aws/platform-engineering/terraform/serverless/iac/2022/08/18/terraform-vs-serverless.html)


Question 5 - In what scenarios would you recommend using Serverless Framework over Terraform, and vice versa?

Answer - Should an organization is having application specific infrastructure, the use of Serverless Framework is preferred.
On the other hand, if an organization is having shared infrastructure, Terraform is preferred. 

Reference: The definitive guide to using Terraform with the Serverless Framework (https://www.serverless.com/blog/definitive-guide-terraform-serverless)


Question 6 - Are there scenarios where using both together might be beneficial?

Answer - If there is shared infrastructure (for example, a shared database) and a few Serverless applications that rely on the shared infrastructure (for example, the Serverless applications create tables in the shared database). In this case, Terraform can be used to manage the shared infrastructure and Serverless Framework can be used to manage the Serverless applications, for example, application deployment and teardown. 

Reference: The definitive guide to using Terraform with the Serverless Framework (https://www.serverless.com/blog/definitive-guide-terraform-serverless)

