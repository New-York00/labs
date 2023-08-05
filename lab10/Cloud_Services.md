# Research Artifact Registries AWS, GCP, and Azure
Each service is designed to be fully integrated with your cloud provider's ecosystem.
The choice may depend on preferences and a registry of artifacts required for current tasks.
Artifacts should also provide full integration with the current landscape of your software.
Each service provides automatic security scanning, additional authentication, access control, and more.

## Azure Artifact Registries

### Azure Artifacts

1) Create and share Maven, npm, NuGet, and Python package feeds from public and private sources
Add fully integrated package management to your continuous integration/continuous delivery (CI/CD) pipelines with a single click
2) Artifacts organized 
Share code effortlessly by storing Maven, npm, NuGet, and Python packages together. And there's no need to store binaries in Git—simply store them using Universal Packages.
3) Protect your packages
Keep every public source package you use—including packages from npmjs and nuget.org—safe in your feed where only you can delete it, and where it's backed by the enterprise-grade Azure SLA.
4) Use with favorite tools (VsCode, IntelliJ IDEA, Atom adn etc)

### Azure Container

1) Geo-replication to efficiently manage a single registry across multiple regions
2) Automated container building and patching including base image updates and task scheduling 
3) Integrated security with Azure Active Directory (Azure AD) authentication, role-based access control, Docker Content Trust, and virtual network integration
4) Integrated with Azure Kubernetes Service and other Azure services

## AWS Artifact Registries

### AWS Container

1) Managed with Docker container images
2) Integrated with other AWS services like ECS and EKS
3) Authorization token. Client must authenticate to Amazon ECR registries as an AWS user before it can push and pull images
4) Can control access to your repositories and the images within them with repository policies.
5) Cross-Region and cross-account replication makes it easier for you to have your images where you need them.
6) Image scanning helps in identifying software vulnerabilities in your container images. Each repository can be configured to scan on push. This ensures that each new image pushed to the repository is scanned.

### AWS Artifacts

1) Integrated with other AWS services
2) Docker support
3) Amazon ECR stores both the containers you create and any container software you buy through AWS Marketplace
4) Amazon ECR stores your container images and artifacts in Amazon Simple Storage Service (S3)
5) Amazon ECR supports the ability to define and organize repositories in your registry using namespaces. This allows you to organize your repositories based on your team’s existing workflows. 

## GCP Artifact Registries

### GCP Artifacts

1) Automate building and deployment.
Automatically build and upload artifacts to private repositories when you commit code to Cloud Source Repositories
2) Native artifact format support.
Create multiple repositories under a given Google Cloud project. Push and pull Docker images, Maven, and npm packages from your private repositories in Artifact Registry using standard command-line interfaces.
3) Secure and consistent.
Set up secure private-build artifact storage on Google Cloud in minutes. Maintain control over who can access, view, or download artifacts with registry-native IAM roles and permissions. 
4) High performance and availability.
Create regional private repositories around the world and store artifacts close to your compute instances anywhere Google Cloud is available. Access Google’s high-performing global network for fast workload delivery.

### GCP Container

1) Container-native networking. Google provides the Kubernetes Defined Network—a network that is fully integrated with GKE. This means easy-to-use integrations with load balancing, routing, security, and network observability. 
2) Defense in depth for Kubernetes. Google Cloud gives you the ecosystem you need to develop and roll out software faster without compromising security; With GKE, you can uniformly and seamlessly establish policy guardrails and let the system declaratively enforce them for you.
3) Allows artifacts to be deployed to Google Cloud runtimes, including Google Kubernetes Engine, Cloud Run, Compute Engine, and App Engine.
4) Automatic security scanning of container images using artifact analysis.

# Research Best Serverless Computing Platforms AWS, GCP, and Azure

Serverless is a way to deploy applications by running functions on-demand. The major advantage of serverless is that it allows an application, or part of an application, to be executed whenever it is needed, but without requiring an execution environment to be running constantly.

In this way, serverless execution models can help to save money. Rather than maintaining a server 24/7 (but only using it part of the time), organizations can deploy code in a serverless environment and pay only for the resources that they actually consume.

1) AWS Lambda
- Lambda supports the execution of functions written in Node.js, Python, Java, C#, and Go. Lambda functions run on shared servers, but each execution environment is isolated; in this respect, Lambda offers similar privacy and security to standard EC2 virtual servers.

2) Azure Cloud Functions
- Some function the same that in AWS Lambda. But support for a broader range of languages: C#, Javascript and F# are currently fully supported on Azure Functions, while Java, Python, PHP, TypeScript, Batch, Bash and PowerShell are available in experimental or preview modes. This makes Azure’s list of supported languages for serverless longer overall than that of AWS Lambda, although the list of available languages is shorter.
- The ability to create and execute stateful serverless functions using the Durable Functions feature on Azure.

3) Google’s Cloud Functions Serverless Platform
- In general, Google Functions is a less mature serverless framework than the serverless platforms from AWS and Azure.
Because it is JavaScript is the only supported language on Google’s serverless platform and possible to execute other languages, such as Python, using third-party wrappers.

4) IBM OpenWhisk
Similar with AWS Lambda

# Links.
1. https://learn.microsoft.com/en-us/azure/container-registry/container-registry-concepts
2. https://azure.microsoft.com/en-us/products/container-registry
3. https://learn.microsoft.com/en-us/azure/container-registry/
4. https://docs.aws.amazon.com/?nc2=h_ql_doc_do
5. https://cloud.google.com/artifact-registry
6. https://aws.amazon.com/lambda/
7. https://docs.microsoft.com/en-us/azure/azure-functions/durable-functions-overview
8. https://azure.microsoft.com/en-us/services/functions/
9. https://cloud.google.com/functions/
10. https://www.ibm.com/cloud/functions