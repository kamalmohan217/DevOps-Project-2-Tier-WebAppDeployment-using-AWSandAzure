# DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure

![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/d2d03d95-bcd7-4b72-bcc8-9505fd9ecf7a)
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
<br><br/>
Add endpoint, username and password of MySQL RDS to the file login.jsp and userRegistration.jsp as shown in the screenshot below
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e664e1b4-5af3-4ab8-ad34-16ee7a2405ce)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/05daa593-e47d-4606-9b84-eddf14fe5565)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/e3ef3a7b-1047-42e5-9008-dafee107cc5e)








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
```
