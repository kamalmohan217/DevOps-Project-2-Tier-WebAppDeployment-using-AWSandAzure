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
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/92b44a14-7404-4109-97a5-f82ff36302ab)
<br><br/>
**To Send Notification on Group Email ID go project Settings or Organisation Settings (For Global Notification) then got to Notifications and New Subscription and create a new Subscription with custom Email ID**
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/507bd24f-197e-4c89-a405-ea56da846c28)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/23477dd6-205b-469b-96a5-94f1951b1f68)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/f05a4102-ce5c-4fd9-bd3b-0c93c819e68e)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/9166cd31-17bd-4c8a-8708-5a9dfcc0a5a0)
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/674e32b9-2280-4296-9550-b83fcca969a7)
