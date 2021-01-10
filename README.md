# ansible
contains Ansible ad-hoc commands and playbooks
## ad-hoc Ansible commands
```
ansible localhost -m ping
...
ansible localhost -m stat -a "path=/ansible"
...
ansible all -i <Public Ip Address>, -m ping -e \
"ansible_user=ansible ansible_password=<Password> ansible_ssh_common_args='-o StrictHostKeyChecking=no'"
...
ansible all -i <Public Ip Address>, -m win_ping -e \
"ansible_user=ansible ansible_password=<Password> ansible_winrm_server_cert_validation=ignore ansible_connection=winrm"
```
