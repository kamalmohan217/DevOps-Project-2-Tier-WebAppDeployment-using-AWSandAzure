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
