sudo apt-get install -y kubelet=1.29.0-1.1 kubeadm=1.29.0-1.1 kubectl=1.29.0-1.1

sudo apt-get install -y kubelet=1.29.0-1.1 kubeadm=1.29.0-1.1 kubectl=1.29.0-1.1

sudo apt-get install -y kubelet=1.29.0-1.1 kubeadm=1.29.0-1.1 kubectl=1.29.0-1.1


kubeadm init --apiserver-cert-extra-sans=controlplane --apiserver-advertise-address 192.32.4.12 --pod-network-cidr=10.244.0.0/16
kubeadm init --apiserver-cert-extra-sans=controlplane --apiserver-advertise-address 192.10.58.9 --pod-network-cidr=10.244.0.0/16

kubeadm join 192.10.58.9:6443 --token 5yj69i.e8k9fhvhjlhed1gi \
        --discovery-token-ca-cert-hash sha256:a1f93c0b7c1b06574337ab1247bcb4f3b0906df61b2e487c4334c604b91780fc
