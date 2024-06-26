# DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure

![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/25024dff-2af4-4bc4-b907-e15ab36d0039)
<br><br/>
**Connection between AWS and Azure using SIte-to-Site VPN**
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/1df759d5-81ab-4107-8dcf-ae6b4952f924)

<br><br/>
**Create Secret to be used for pull image from Azure ACR**
```
kubectl create secret docker-registry devopsmelacr132827a7-auth --docker-server=https://akscontainerregistry2405.azurecr.io --docker-username=akscontainerregistry2405 --docker-password=iXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXp -n demo
```
**Create Secret for tls cerficates to be used in Ingress Rule**
```
kubectl create secret tls ingress-secret --key mykey.key --cert STAR_singhritesh85_com.crt -n demo
```
<br><br/>
**Follow below steps to make your Azure DevOps Agent ready.**
<br><br/>
Install git2 
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/f4a4c238-924c-4d30-883c-d364d177aaaa)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/966f7f0f-54e3-4967-96a1-c782a32d73fd)
Create a user demo and provide sudo privileges from sudoers file.
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/fc91bffa-9b8f-49b8-94ba-cf1a111ff178)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e5f4de24-410a-44a8-aa5a-69c6179568d5)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/91d27281-d0d7-4781-a351-d1ba0bfa3fcb)
Install Java-17
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/dd88df36-5ec1-411e-9922-1df81c6078dd)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3a5e14a5-344d-455b-82c3-26c58f21204d)
Install maven
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e6dcd6e9-0b2f-49b1-80a2-ba623b011641)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/9bba2d80-a8ff-48c7-83ec-448df1c36f9b)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3db44693-814e-42bd-813f-daf72551ce00)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/033440bd-dbbf-49f2-b109-a216433123de)
<br><br/>
Install Docker
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/48b55f93-a0f4-4f37-81e4-0e0e58582458)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/1b266eac-f173-4e0c-b07b-72c3b4c28d79)
<br><br/>
Install self hosted agent pool (You can create self hosted agent pool either at Organisation level or at project level)
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/d72dc8be-82a3-47b9-93f6-e7be4e7fbdc7)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/c76d1a11-d7b6-4dd8-be14-9ce4fc8fe367)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/045054dc-6e72-4eb3-a395-feef2dd2f321)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3789adb8-db12-4c82-9812-07d29e1ef11f)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3707afa6-0844-4c9e-a24c-f6293dec9d15)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/4f21b984-5f5a-4a56-8745-45f79190d590)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/77df105d-6f86-455e-a24b-5edb1e800431)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/b2fa72f1-b9ef-478a-ad2c-e43df2748050)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/5e209c12-6f24-4532-abaf-72d1e67c254d)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/7aef2609-ee9f-4ae7-b56a-dbb3fe060363)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/bb8a4840-9ead-44ea-9126-b3a7d7d059a4)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/af0a5c8a-0dd0-4d63-ae19-81b5a981aa69)
<br><br/>
Copy kubeconfig from Terraform-Server to Azure DevOps Self-Hosted Agent and Install kubectl and helm
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/c95869af-b779-42c3-a14b-3e7e3b280602)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/78d896be-35e5-4a17-a241-0d1d8a1eb8f2)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/01213bb2-c5d6-42e0-8eba-a1a8dc1b5fc4)
<br><br/>
Install trivy for Docker Image Scan
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/9685fe88-425a-42b2-b64c-82acb2ecdacc)

<br><br/>
Create three service connections as shown in the screenshot below
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/631cf1dd-d06e-4128-a836-a95a5d157581)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/b0dd1460-3c57-47db-81dd-094280fa9b43)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/b4380144-ffb2-449e-869f-0ee5d25ee5d7)
<br><br/>
**To Send Notification on Group Email ID go project Settings or Organisation Settings (For Global Notification) then got to Notifications and New Subscription and create a new Subscription with custom Email ID**
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/507bd24f-197e-4c89-a405-ea56da846c28)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/23477dd6-205b-469b-96a5-94f1951b1f68)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/f05a4102-ce5c-4fd9-bd3b-0c93c819e68e)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/9166cd31-17bd-4c8a-8708-5a9dfcc0a5a0)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/674e32b9-2280-4296-9550-b83fcca969a7)
<br><br/>
Adding below lines to pom.xml for storing Artifacts to Azure Artifactory
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/04384dea-8937-42d1-8e90-9a8ae0a611ef)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/15704438-2b62-4906-94ba-94ed4fa5052a)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3192ac04-9e89-4d5e-9e04-7e6c588d52f1)

<br><br/>
Add endpoint, username and password of MySQL RDS to the file login.jsp and userRegistration.jsp as shown in the screenshot below
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e664e1b4-5af3-4ab8-ad34-16ee7a2405ce)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/05daa593-e47d-4606-9b84-eddf14fe5565)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e3ef3a7b-1047-42e5-9008-dafee107cc5e)
<br><br/>
**Prometheus and Grafana Configuration**
<br><br/>
Using Terraform Script Prometheus and Grafana has been installed and Prometheus is kept as a source for Grafana.
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/81346f68-6a80-49a4-8d22-b68505b97dc4)
<br><br/>
Dashboard has been imported using the ID **3119** as shown in the screenshot below
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/7ec41be4-b110-4f97-a890-7ae35502a166)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/43a98b56-bf29-4e20-8f83-dffbe8920a95)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/09575cdd-e4e6-4632-bd89-2c1b121a6841)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/0e48ae18-bc44-4dde-b454-64298715df7d)
<br><br/>
You can access the application as shown below
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/1797d1b1-0822-4e76-b7b5-de9cbc2ac705)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/8e3cac0f-5c7e-40c1-befe-10b7a82d75ce)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/3f0dfca4-af74-42da-9c89-4e20ac841852)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/5e151bad-b355-495f-81e9-9407ef754238)








<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
<br><br/>
**Reference:-** 
**Reference:-** 
```
https://ashok198510.hashnode.dev/cloud-native-two-tier-application-deployment-with-eks-tomcat-and-rds-in-aws
https://github.com/Ashoksana/aws-rds-java
https://medium.com/@abiolamajekodunmi2011/implementing-secure-and-observant-3-tier-deployments-on-aws-using-terraform-eks-jenkins-ea2572d239e1
```
