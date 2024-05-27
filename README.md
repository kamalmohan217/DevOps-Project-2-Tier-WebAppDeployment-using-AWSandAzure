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
Create three service connection as shown in the screenshot below
<br><br/>
![image](https://github.com/kamalmohan217/DevOps-Project-2-Tier-WebAppDeployment-using-AWSandAzure/assets/128888356/631cf1dd-d06e-4128-a836-a95a5d157581)
