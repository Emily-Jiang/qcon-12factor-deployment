# QCon 12 Factor App Deployment
This repo is about how to deploy the two 12 Factor APP microservices to Kubernetes.
Checkout this gitrepo and cd to the directory where the deployment.mf lives and issue the following command
```
  kubectl apply -f deployment.mf

  kubectl get pods
  
  When you see the following:
  emilyjiang@Emilys-MBP Deployment % kubectl get pods
NAME                                         READY   STATUS    RESTARTS   AGE
12factor-app-a-deployment-7c85569d77-2qmv4   2/2     Running   0          26s
12factor-app-a-deployment-7c85569d77-xmlm8   2/2     Running   0          26s
12factor-app-b-deployment-649f7f7c78-fwvqt   2/2     Running   0          26s
12factor-app-b-deployment-649f7f7c78-m6qql   2/2     Running   0          26s
```

Test your microservices by hitting the following url
http://localhost:30080

You should see the welcome page and each link should work.
Hope you have enjoyed the journey towards 12 Factor App!
