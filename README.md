# ansible_role_provision_test_docker

```bash
sudo apt-get update -y
sudo apt install -y python3-pip
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install -y ansible sshpass
ansible-galaxy collection install community.general

sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/$(echo "$(lsb_release -is)" | tr '[:upper:]' '[:lower:]') $(lsb_release -cs) stable"
sudo apt-get update -y
sudo apt-get install -y docker-ce docker-ce-cli containerd.io
```