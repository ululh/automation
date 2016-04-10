# Ansible to deploy Hadoop (HDP) on Ubuntu containers

Ansible playbooks for HDP (Hortonworks Hadoop) on Ubuntu containers 
To play on an Ubuntu host

For roles includes : set roles_path    = /etc/ansible/playbooks/roles in ansible.cfg

python-lxc that comes in Ubuntu 15.10 doesn't work : you need to install lxc-dev from apt-get and then install lxc-python2 through pip or by downloading zip
