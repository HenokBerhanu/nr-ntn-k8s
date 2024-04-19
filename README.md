# 2 Node kubeadm cluster on VirtualBox

Its a two node kubernetes cluster (master and worker)

Node IP Cidr = 192.168.56.0/24

clone the repo: https://github.com/HenokBerhanu/nr-ntn-k8s.git

Install vagrant and virtualbox in your host.

vagrant up # this command will set up a two node VM for the k8s cluster

For the kubernetes installation:  got to this directory /nr-ntn-k8s/ubuntu/vagrant

# Got this file run the code blocks in both master and worker nodes:
             /nr-ntn-k8s/ubuntu/vagrant/node-setup.sh
# For setting the k8s master node: use the file below:
              /nr-ntn-k8s/ubuntu/vagrant/controlplane.sh
    
    
# Description about the k8s cluster:
          CNI: flannel with pod cidr of 10.244.0.0/16
          Has RBAC support
          Master node IP: 192.168.56.120
          Worker node IP: 192.168.56.102
