# Redis_Ansible


Change var file with your password:

REDIS_PASSWORD: ********

Change servers in inventory:

server-01 ansible_host=xxx.xxx.xxx.xxx role=master

server-02 ansible_host=xxx.xxx.xxx.xxx role=replica

server-03 ansible_host=xxx.xxx.xxx.xxx role=replica

## Getting started

1. Create 3 servers with public-key authentication
2. Copy `vars.yml.example` to `vars.yml`. Replace `<YOUR_PASSWORD>` with a secured password
3. Edit `inventory` file and replace `<SERVER_01_IP>`, `<SERVER_02_IP>` and `<SERVER_03_IP>` with the corresponding IP address for each server.
4. Run playbook `setup-redis-sentinel.yml`

    ```bash
    ansible-playbook setup-redis-sentinel.yml -i inventory -K
    ```

