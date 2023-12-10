# Redis_Ansible


## Getting started

1. Create 3 servers with public-key authentication
2. In `vars.yml`. Replace `<YOUR_PASSWORD>` with a secured password
3. Edit `inventory` file and replace `<SERVER_01_IP>`, `<SERVER_02_IP>` and `<SERVER_03_IP>` with the corresponding IP address for each server.
4. Run playbook `setup-redis-sentinel.yml`

    ```bash
    ansible-playbook setup-redis-sentinel.yml -i inventory -K
    ```

