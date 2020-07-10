## LAMP stack with Ansible
Here, in this project, I explain how to use Ansible to automate installing LAMP stack on a server and run an application.  

For this tutorial, I use a Centos box provisioned by Hashicorp Vagrant and VirtualBox. You can use VirtualBox and VMware directly, but I prefer to use Vagrant as it gives me more features to configure my virtual machine. 

In this tutorial, I used the application developed by KodeKloud team [here](https://github.com/kodekloudhub/learning-app-ecommerce/tree/master). The instruction to run this application on a server with LAMP stack is provided on the application folder. 




## LFMP stack with Ansible



Add below to vagrant_ansible_inventory. This is the auto-generated inventory file by Vagrant and it encompasses all of the virtual machines it manages, and use it for provisioning machines.

default ansible_ssh_host=127.0.0.1 ansible_ssh_port=2222 ansible_ssh_user='vagrant' ansible_ssh_private_key_file='/home/mostafa/DevOps studies/Ansible/.vagrant/machines/default/virtualbox/private_key'