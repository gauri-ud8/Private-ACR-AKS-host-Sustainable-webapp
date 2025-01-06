# Private-ACR-AKS-host-Sustainable-webapp
Empowering cloud-native deployment with private AKS and ACR to host a sustainability application!

Thrilled to share an incredible project I recently developed, where I designed and implemented a secure, scalable CI/CD pipeline for cloud-native applications! 
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
This project was an exciting opportunity to build a production-ready solution that balances efficiency, scalability, and security. This project truly presented a challenge to in novate and deliver cutting-edge solutions.
![792a725a-8556-4b12-83a6-d7d2ac97633d](https://github.com/user-attachments/assets/1bf43939-8e92-4664-ace2-3a84662f934b)
![ba39be39-9366-49dd-becf-876a83aff47f](https://github.com/user-attachments/assets/c34563ea-777f-4b3a-9f09-bdcd53a630fa)
![6045b667-50e8-4b81-846c-bcdc46c05a8b](https://github.com/user-attachments/assets/13a98bf5-7d9a-4bd4-81cf-8b6e89ed483d)
![2642cf04-9610-46d7-beba-5b6958f277ad](https://github.com/user-attachments/assets/53cf21f0-c5be-4542-951e-91fb9c6ec409)
![33771710-0fae-4611-8d93-04aa88442a5f](https://github.com/user-attachments/assets/d4698b3e-789f-40bd-9b14-510213a4549d)
![4677b71a-4883-424f-b8d2-3627ee0dc803](https://github.com/user-attachments/assets/0d1eb7be-33e7-42f7-b9a8-594768ea0904)
![9271e923-93be-402f-bf61-d9a8def5ecb9](https://github.com/user-attachments/assets/c754edcd-1295-45d6-8756-42f65d6bebd8)
