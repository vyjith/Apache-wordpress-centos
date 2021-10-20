# Installing wordpress using ansible on cetnos

# **Description**
-------------------------------------------------- 

Here we are going to create a wordpress site using the ansible on centos machine. 

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

