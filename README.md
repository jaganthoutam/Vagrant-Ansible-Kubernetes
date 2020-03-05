# vagrant-ansible-kubernetes
Combination of Vagrant and Ansible to spin up a Kubernetes cluster

### Prerequisites
- Vagrant 2.1.4+
- Virtualbox 5.2.18

### Define amount of nodes
in Vagrantfile:
```
N = 2
```


### Spin up cluster
```
$ vagrant up
```

### Verify on master
```
vagrant@k8s-master:~$ kubectl get no
NAME         STATUS   ROLES    AGE   VERSION
k8s-master   Ready    master   17h   v1.14.0
node-1       Ready    <none>   17h   v1.14.0
node-2       Ready    <none>   17h   v1.14.0
```
