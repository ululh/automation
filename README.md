# automation

Ansible scripts


Prereq when deploying on Raspberry Pi :

install or clone Dietpi (http://dietpi.net/) on every participating raspberry Pi node

Ansible prereq : 

    On controller :
        Install Ansible
        scp_if_ssh = True in /etc/ansible/ansible.cfg (or whereever conf file is located, that's because there is no sftp in dropbear, dietPi ssh server)
        generate private/public key pair
    On managed R Pi : 
        put ssh public key in /root/.ssh/authorized_keys
        mv /etc/motd /etc/motd.orig
        apt-get install python
        apt-get install openssh-client
