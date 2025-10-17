This is complete initial stack to setup your N8N instance with postgres database for long term memory 
and Qdrant vector database for embeddings to store.

Steps:

1- update your system

sudo apt update && sudo apt upgrade -y

2- install latest version of docker

sudo apt install apt-transport-https ca-certificates curl software-properties-common

sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc

sudo apt update

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update

sudo apt install docker-ce

sudo apt install git


