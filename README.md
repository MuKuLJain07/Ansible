# Ansible
̌Ansible is an open-source IT automation tool that automates tasks like provisioning, configuration management, application deployment, and orchestration

### Difference between Ansible and Terraform
Terraform is used to create infrastructure, it is a code as an infrastructure tool whereas ansible is used to patch and manager those infra.

### Difference between Chef and Ansible
 - Both are configuration management tool
 - Chef uses pull based mechanism whereas Ansible uses push based mechanism.

## Installing Ansible
```
brew update
brew install ansible

brew --version
```

The /etc/ansible/hosts file is Ansible's inventory, where it locates the machines it manages
```
sudo mkdir -p /etc/ansible
sudo touch /etc/ansible/hosts
```

Now add the below into your /etc/ansible/hosts file
```
[ec2]
52.66.21.22 ansible_user=ubuntu ansible_ssh_private_key_file=~/.ssh/id_rsa
```
where id_rsa is your system's private key

## Ansible Commands
1. Ad Hoc Commands: 
Ansible ad hoc commands are quick, simple instructions you can give to many computers at once. They are like short messages you can send to lots of computers, telling them to do one small task right away.
2. Ansible playbook