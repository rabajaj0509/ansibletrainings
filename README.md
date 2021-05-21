# Automation-with-Ansible:

This is a beginners Ansible tutorial. It consists of few excercises
that illustrate the following topcs:

1) Ansible Inventory
2) Playbooks
3) Modules
4) Variables
5) Conditionals
6) Loops
7) Roles

The repository contains many questionnaires, problem statements
and quizs for the attendees of the worshop. So feel free to open
new pull-requests!

I have used these labs for performing my workshop at various conferences 
and college fests like:

1) [###rootconf 2018.](https://rootconf.in/2018-automation-with-ansible/)
2) Persona Fest' 2019.

## Setup


### Clone the repository
```
$ git clone https://github.com/rabajaj0509/ansibletrainings.git
$ cd set-up
```

### Install Vagrant
```
$ sudo dnf install vagrant-libvirt
$ sudo dnf install @vagrant
$ sudo systemctl enable libvirtd
```

### Usr vagrant without being asked for password for each command
```
$ sudo gpasswd -a ${USER} libvirt
$ newgrp libvirt
```

### Using vagrant
```
$ vagrant status
$ vagrant up
```

Once both the machines are up and running (check vagrant status), you 
will need to manually create ssh keys on the control node, you can do 
this by:

```
$ ssh-keygen -t rsa
``` 

And, last step, you need to copy the public key of the controlnode into the 
authorized_keys file of the managednode. Also, if you want to use the nodes 
by their names, then dont forget to add the managednode's entry in /etc/hosts
file of the controlnode. For better understanding of the setup you can also 
refer to this [document](https://github.com/rabajaj0509/ansibletrainings/blob/master/Ansible-Configuration.png)

I hope this set-up is helpful.
