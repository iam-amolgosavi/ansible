# Referrencing purpose if multiple linux machines like Unutu,amazonlinux,redhat 
# /etc/asible/hosts file

```
[ubuntu_servers]
ubuntu_host1 ansible_host=3.149.239.98
ubuntu_host2 ansible_host=13.59.51.63

[amazonlinux_servers]
amazon_host1 ansible_host=54.123.45.67
amazon_host2 ansible_host=18.98.76.54

[redhat_servers]
redhat_host1 ansible_host=192.168.1.100
redhat_host2 ansible_host=192.168.1.101

[ubuntu_servers:vars]
ansible_user=ubuntu
ansible_ssh_private_key_file=/home/ubuntu/keys/ubuntu-key.pem
ansible_python_interpreter=/usr/bin/python3

[amazonlinux_servers:vars]
ansible_user=ec2-user
ansible_ssh_private_key_file=/home/ubuntu/keys/amazonlinux-key.pem
ansible_python_interpreter=/usr/bin/python3

[redhat_servers:vars]
ansible_user=root # or a specific user on your redhat machines.
ansible_ssh_private_key_file=/home/ubuntu/keys/redhat-key.pem
ansible_python_interpreter=/usr/bin/python3```
