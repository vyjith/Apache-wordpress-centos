# Installing wordpress using ansible on cetos 7

# **Description**
-------------------------------------------------- 

In this guide, we’ll focus on getting a Wordpress 5.7.2 instance set up on a LAMP stack (Linux, Apache, MySQL, and PHP7.2) on an Cetnos 7 server.

# Prerequisites

- Master server installed with [Ansible2](https://docs.ansible.com/ansible/2.3/index.html) (For your reference visit [How to install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html))
##### Ansible Modules used:
[Inventory](https://docs.ansible.com/ansible/2.3/intro_inventory.html) , [File](https://docs.ansible.com/ansible/2.3/list_of_files_modules.html), [Database](https://docs.ansible.com/ansible/2.3/list_of_database_modules.html), [Command](https://docs.ansible.com/ansible/2.3/list_of_commands_modules.html)

# How to Use:

First create a directory in master server. Then, clone this Github repository [apache_wordpress_cents](https://github.com/vyjith/Apache-wordpress-centos) to your maset server which is per-installed with Anisble-2. Once you cloned this repository, edit your "hosta" file [invenetory file](https://docs.ansible.com/ansible/2.3/intro_inventory.html) accordingly. 

Check the connection status to your client server via:
```
ansible -i hosts webserver -m ping

```
Once you have established connection, then check if any syntax error in the playbook using the following command
```
ansible-playbook -i hosts wordpress.ym --syntax-check
```
If you are good to go, then execute the anible playbook
```
ansible-playbook -i hosts main.yml
```

Secuity Feuture
-------------------------------------------------- 

After the installation, inorder to imporve the security, pleasae change the mysql credentials and also change the credentils in the wp-config.php file
Additionlaly, here I have used plain mysql credentials, you can encrypt the credentials using the [ansible vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html)

### ⚙️ Connect with Me
<p align="center">
<a href="https://www.instagram.com/iamvyjith/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/vyjith-ks-3bb8b7173/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
