# Proxmox version-7 ansible repo

1. Ansible must be installed in the environment
2. Ansible will configure a cron-job that watches this repo for changes if any changes made ansible will automatically update the configuration in every machine 

<!-- ## Run this command as a root user to install and run ansible
```sh
curl 172.16.16.65:8081/ansible/ | bash
  ```
The above command downloads a bash file from 172.16.16.65 and runs the following commands instead of running one by one -->

## Run the below command incase if the above command fails

```sh
apt update -y;
apt install git ansible -y;
ansible --version;
ansible-pull -U https://github.com/nobixX/ansible-docker.git proxmox.yml;
  ```

