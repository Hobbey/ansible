### Ansible Playbook

Documentation Ansible:
http://docs.ansible.com/ansible/playbooks_best_practices.html

\# install ansibe use ppa

```
apt-get install software-properties-common
apt-add-repository ppa:ansible/ansible
apt-get update
apt-get install ansible
```

\# init server (put sys_ansible private key into ~/.ssh/sys_ansible)

```
alias ap='ansible-playbook'
ap server_setup1_init.yml -i inventory_SH -l init -k -K -s -e ansible_ssh_user=ops
ap server_setup2_basic.yml -i inventory_SH -l init
ap server_setup3_docker.yml -i inventory_SH -l init
```

\# AAA
