# ansible_napalm
Installation: 

sudo apt-get update && sudo apt-get install software-properties-common 
sudo apt-add-repository ppa:ansible/ansible 
sudo apt-get update 
sudo apt-get install ansible

To Install napalm-Ansible:

pip install napalm-ansible
touch ~/.ansible.cfg

$ napalm-ansible -h
To ensure Ansible can use the NAPALM modules you will have to add the following configurtion
to your Ansible configuration file (ansible.cfg):
    [defaults]
    library = /usr/local/lib/python2.7/dist-packages/napalm_ansible/modules
    action_plugins = /usr/local/lib/python2.7/dist-packages/napalm_ansible/plugins/action

For more details on ansible's configuration file visit:
https://docs.ansible.com/ansible/latest/intro_configuration.html
