**Ref:** https://www.youtube.com/watch?v=6kmHvXdAzIM&t=426s&ab_channel=ThatDevOpsGuy

step:
- make docker image for suitable storage/os/cluster. es example is given in this repo
- deploy es-kibana stack in cluster
- deploy rbac,config map for fluentd custom configuration and fluentd demon set

fact:
- log files path could be differnt for differrent cluster/system. We need to mount appropiet path to the demonset. Like for Kind, Kubelet store logs in /var/log path.