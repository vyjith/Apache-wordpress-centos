# Installing wordpress using ansible on cetos 7

# **Description**
-------------------------------------------------- 

In this guide, we’ll focus on getting a Wordpress 5.7.2 instance set up on a LAMP stack (Linux, Apache, MySQL, and PHP7.2) on an Cetnos 7 server.

# Edit the hosts file and add your server IP following is the one example of the hosts file entry

-------------------------------------------------- 

```
[webserver]

192.168.178.15
192.168.178.16

[Databse]

192.168.178.18
192.168.178.19
```

# Run the following command for running the playbook

```
anible-playbook wordpress.yml
```

### ⚙️ Connect with Me
<p align="center">
<a href="https://www.instagram.com/iamvyjith/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/vyjith-ks-3bb8b7173/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
