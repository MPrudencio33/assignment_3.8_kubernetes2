# assignment_3.8_kubernetes2
Answer to Assignment on Module 3.8 Kubernetes Part 2

# <to display the namespaces>
zanjero@ZANJERO:~/activity3.8_kubernetes2$ kubectl get namespace
NAME                    STATUS   AGE
alfatah-eks-activity    Active   32m
andyhtc-eks-activity    Active   39m
angeline-eks-activity   Active   61m
dave-eks-activity       Active   19m
default                 Active   4h30m
jiaqing-eks-activity    Active   22m
kube-node-lease         Active   4h30m
kube-public             Active   4h30m
kube-system             Active   4h30m
luqman-eks-activity     Active   61m
marlon-eks-activity     Active   42m
ninadc-eks-activity     Active   26m
saw-eks-activity        Active   96m
shilpa-eks-activity     Active   33m
siti-eks-activity       Active   27m
sree-eks-activity       Active   27m
sridhar-eks-activity    Active   45m
test-eks-activity       Active   65m
tssohn-eks-activity     Active   58m
vimal-eks-activity      Active   70m
yeefei-eks-activity     Active   40m

#Show that your resources (ConfigMap/Secrets/Services) are deployed within your #namespace

zanjero@ZANJERO:~/activity3.8_kubernetes2$ kubectl get svc -n marlon-eks-activity
NAME                          TYPE           CLUSTER-IP       EXTERNAL-IP                                                               PORT(S)           AGE
marlon-clusterip-service      ClusterIP      10.100.105.128   <none>                                                                    8080/TCP          14m
marlon-loadbalancer-service   LoadBalancer   10.100.151.56    a2f47c22dc88a4ea3a6913b5aa44cf3b-1893798715.us-east-1.elb.amazonaws.com   80:31582/TCP      15m
marlon-nodeport-service       NodePort       10.100.7.4       <none>                                                                    30001:32410/TCP   14m