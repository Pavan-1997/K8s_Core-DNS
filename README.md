# K8s_Core-DNS

1. Curl the Nginx (Localhost) 
```
k exec -it nginx -- curl nginx
```
![image](https://github.com/user-attachments/assets/128ffe60-4e29-47cb-b3e0-2b8042eaa271)


2. Check the Services
```
k get svc -n=kube-system
```
![image](https://github.com/user-attachments/assets/4be0696e-1c92-43d0-9a79-ba2e12cf316e)


3. Check the Files fo DNS inside the Pod - Login to the Nginx Pod to check the Local DNS

![image](https://github.com/user-attachments/assets/1a171ce4-0acb-4155-9327-63a693147c1c)


4. In this we can add another IP of POD to reach 

![image](https://github.com/user-attachments/assets/0c77f0e5-2a08-4007-af39-e528c9f1f343)


5. Important file to check for Core DNS

```
k describe cm coredns -n=kube-system
```
