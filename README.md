# Quorum Blockchain Setup

## Commands
```
  curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
  chmod +x ./kubectl
  sudo mv ./kubectl /usr/local/bin/kubectl
  sudo apt-get update && \
      sudo apt-get install docker.io -y

  sudo apt-get install -y conntrack
  cd /usr/bin/
  ln -s /usr/sbin/conntrack conntrack

  curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
  minikube version
  minikube start --vm-driver=none
  wget https://dl.google.com/go/go1.16.4.linux-amd64.tar.gz 
  sudo tar -xvf go1.16.4.linux-amd64.tar.gz   
  sudo mv go /usr/local 
  export GOROOT=/usr/local/go 
  export GOPATH=$HOME/Projects/Proj1 
  export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
  go version
  GO111MODULE=on go get github.com/ConsenSys/qubernetes/qctl
  qctl --help
```

## Links
- [Quorum](https://consensys.net/quorum/developers/)
- [Qubernetes](https://docs.goquorum.consensys.net/en/stable/GetStarted/Getting-Started-Qubernetes/)
