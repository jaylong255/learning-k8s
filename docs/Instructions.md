# Instructions

[Go Home](https://github.com/jaylong255/learning-k8s)

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

## Installing kubectl from binaries, Linux

Download the latest release.

    curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

Download the checksum

    curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"

Validate

    echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check

Install

    sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

Test

    kubectl version --client --output=yaml  


https://www.cloudsigma.com/how-to-install-and-use-kubernetes-on-ubuntu-20-04/

https://stackoverflow.com/questions/36939381/x509-certificate-signed-by-unknown-authority-kubernetes



### test

reset the control plane

    sudo kubeadm reset

initialize control plane

    sudo kubeadm init --ignore-preflight-errors=NumCPU,Mem --pod-network-cidr=10.244.0.0/16

apply the deployment.yaml

    kubectl apply -f deployment.yaml


dfdf

    kubeadm join 192.168.1.240:6443 --token gwriub.89ni1i4ooezjoa3c --discovery-token-ca-cert-hash sha256:daf44a17cb3464a08cfefb0c94750f5efd29bf2483a2742fd6132f3abbbf7e85

