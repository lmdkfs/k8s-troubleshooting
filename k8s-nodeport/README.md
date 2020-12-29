# 调用链
client: 10.0.0.45 --> nodeport 10.0.0.30 --> node 10.0.0.34 --> pod 172.16.2.176

结论:

- clientPort 在nodepor 节点转发是原por端口不变
- 在pod中看到的源ip为nodeport节点ip

![wireshark](image/k8s-nodeport.png)
