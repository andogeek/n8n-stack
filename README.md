This is complete initial stack to setup your N8N instance with postgres database for long term memory 
and Qdrant vector database for embeddings to store.

Get 60days free trial from Digital Ocean

https://try.digitalocean.com/app-platform/?irclickid=0-oyGkWUjxycTu10v%3AQO80UFUkpyswxnK3KL0o0&irgwc=1&utm_campaign=2933979&utm_content=&utm_medium=affiliates&utm_source=impact

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

git clone https://github.com/andogeek/n8n-stack.git

cd n8n-stack

docker compose up -d
