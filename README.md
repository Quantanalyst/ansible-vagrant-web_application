## LAMP stack with Ansible
Here, in this project, I provaide the ansible playbook to automate installing LAMP stack on a server and run an application.  

For this part, I use a Centos box provisioned by Hashicorp Vagrant and VirtualBox. You can use VirtualBox and VMware directly, but I prefer to use Vagrant as it gives me more features to configure my virtual machine. 

In this tutorial, I used the application developed by KodeKloud team [here](https://github.com/kodekloudhub/learning-app-ecommerce/tree/master). The instruction to run this application on a server with LAMP stack is provided on the application folder. 




## LFMP stack with Ansible
Also, the ansible playbook to automate LFMP stack is provided. For this part, I used Debian box. The Vagrantfile for both Centos and Debian are accessable in this folder. 

Note1: in order to define an inventory for the vagrant vm, you can use the auto-generated inventory file by Vagrant. You can access the file in .vagrant/provisioners/ansible/inventory directory. This file gives you the ansible variables you need to define your ansible host. Below is an example of such host.
```
default ansible_ssh_host=127.0.0.1 ansible_ssh_port=2222 ansible_ssh_user='vagrant' ansible_ssh_private_key_file='<your_local_project_folder>/.vagrant/machines/default/virtualbox/private_key'
```