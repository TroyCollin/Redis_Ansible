# Redis_Ansible


Change var file with your password:
Like this:

REDIS_PASSWORD: ********

Change servers in inventory:

server-01 ansible_host=xxx.xxx.xxx.xxx role=master

server-02 ansible_host=xxx.xxx.xxx.xxx role=replica

server-03 ansible_host=xxx.xxx.xxx.xxx role=replica


