# Private-ACR-AKS-host-Sustainable-webapp
Empowering cloud-native deployment with private AKS and ACR to host a sustainability application!

Thrilled to share an incredible project I recently collaborated on with Shubham Hadgal, where we designed and implemented a secure, scalable CI/CD pipeline for cloud-native applications! 
# 🔧 Key Highlights:  
1. Configured a self-hosted Azure DevOps agent within a secure virtual network.  
2. Integrated private Azure Kubernetes Service (AKS) and Azure Container Registry (ACR) with seamless networking.  
3. Deployed SonarQube (using Helm) for automated code quality checks and vulnerability analysis.  
4. Implemented Trivy for container image scanning in the pipeline.  
5. Automated the deployment process using ArgoCD to manage and synchronize application manifests. 
# 💡 The Workflow:  
1. Developers push code changes to Azure Repos, triggering the Azure DevOps pipeline.  
2. Code is scanned for vulnerabilities using SonarQube. If the quality gate passes, a Docker image is built.  
3. The image is scanned with Trivy, ensuring compliance with security standards.  
4. Once verified, the image is pushed to a private ACR configured with VNet peering and DNS resolution.  
5. ArgoCD automatically deploys the application to a private AKS cluster with the latest image.  
6. The application is exposed securely over the Internet via the NGINX Ingress Controller. 
# 🔒 Security Measures:  
1. Used service connections in Azure DevOps to securely access private resources.  
2. Ensured private networking between the DevOps agent, ACR, and AKS using VNet peering and private DNS zones.  
3. Added automated security checks at every stage to maintain code and image integrity.
# 📂 Visuals:
To provide more clarity, the DevOps pipeline workflow diagram and the architectural design showcase the end-to-end implementation and infrastructure in detail.
This project was an exciting opportunity to build a production-ready solution that balances efficiency, scalability, and security. This project truly presented a challenge to innovate and deliver cutting-edge solutions.
