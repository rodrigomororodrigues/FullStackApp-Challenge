# FullStackApp-Challenge

 API-Asp.Net--Mysql-AKS-Terraform

activities:

1. Develop a User Story - Done 
Create an informal user story that outlines the objectives and requirements for deploying the sample API and its database. This user story will guide the development and deployment process, ensuring all components interact correctly and meet the specified criteria.

2. Set Up Terraform Code
Develop Terraform code to provision the necessary Azure resources for the deployment. This should include, but not be limited to, Azure Kubernetes Service (AKS) clusters, networking resources, and any other infrastructure components required for the deployment. Organize the Terraform code to accommodate multiple environments and adhere to best practices in infrastructure as code (IaC).

3. Prepare Helm Charts
Create Helm charts to describe all cluster resource sets needed for the application and its database. If preferred, Kustomize can also be used. Ensure that the Helm charts are well-organized and follow best practices for Kubernetes resource management.

4. Create Dockerfiles
Develop Dockerfiles for the sample API and its database. These Dockerfiles should be optimized for production, ensuring they are secure, lightweight, and adhere to Docker best practices.

5. Implement CI/CD (Optional)
Setting up a Continuous Integration/Continuous Deployment (CI/CD) system to automate the deployment process is an optional but highly recommended step. This could involve integrating with GitHub Actions, Azure DevOps, or any other CI/CD tools you're comfortable with.

6. Add DevOps/SRE Practices (Optional)
Incorporate additional components that demonstrate your understanding of DevOps/SRE practices. This could include monitoring, log management, alerts, and any other operational tools or practices that enhance the deployment's reliability and observability.

7. Presentation and Code Review Preparation
Prepare a presentation that covers the user story, design choices, technical architecture, and functionality of the deployment. Be ready to share your project through a GitHub repository or IDE during a Zoom call with the technical interview panel. Anticipate questions related to your code and be prepared to explain your decisions.

8. Code Quality and Functionality
Ensure that your code is well-organized, readable, and adheres to best practices. The application should function as described, with the API accessible from the outside and the database secured.

By addressing each of these activities, you will be able to create a comprehensive and well-organized approach to the technical interview exercise. Good luck!


# Add  aks extension
- az extension add --name aks-preview
# Add  Container Extension 
az provider register --namespace Microsoft.ContainerService
# Add Update aks Extension
- az extension update --name aks-preview
# Add Network Modules
- az provider register --namespace Microsoft.Network
# Add Container Instance Modules
- az provider register --namespace Microsoft.ContainerRegistry
# Add KeyVault Modules
- az provider register --namespace Microsoft.KeyVault
# Add Cognitive Modules
- az provider register --namespace Microsoft.CognitiveServices
# Add  AKS-KedaPreview Modules
az feature register --namespace "Microsoft.ContainerService" --name "AKS-KedaPreview"
# Add Storage Modules
- az provider register --namespace Microsoft.Storage
# Add Operational Insights Modules
- az provider register --namespace Microsoft.OperationalInsights

# Add Microsoft Insights Modules
- az provider register --namespace Microsoft.Insights

# Add Operations Management Modules
- az provider register --namespace Microsoft.OperationsManagement

# Add Compute Modules
- az provider register --namespace Microsoft.Compute

# to Consult Status from installed modules use the command below

- az provider show --namespace "moduleName" --query "registrationState"
