## goal - configure instance on Nectar / Melbourne Research Cloud

### Step 1
Install ansible

### Step 2
Get the IP address of your cloud instance and edit this in the 'hosts' file. Edit the path to your private ssh key file in the same file. 

### Step 3 
Run the playbook with the following command:
```
ansible-playbook -i hosts nextflow.yaml
```