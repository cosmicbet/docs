# Requirements

## Software Install

```
# System Update
apt update && apt upgrade -y
apt install build-essential git unzip jq -y

# Install golang
wget https://golang.org/dl/go1.16.linux-amd64.tar.gz
sudo tar -xvzf go1.16.linux-amd64.tar.gz
sudo mv go /usr/local

# Update Environment
cat <<EOF >> ~/.profile
export GOPATH=$HOME/go
export GO111MODULE=on
export PATH=$PATH:/usr/local/go/bin:$HOME/go/bin
EOF

source ~/.profile
go version
# go version go1.16 linux/amd64
```