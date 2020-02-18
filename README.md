## goal - configure instance on Nectar / Melbourne Research Cloud

### Step 1
Get the IP address of your cloud instance and edit this in the 'hosts' file in this directory.

### Step 2
Get the IP address of your cloud instance and edit this in the 'hosts' file in this directory.

### Step 3 
Run the playbook with the following command:
```
ansible-playbook -i hosts -u ubuntu --key-file=~/path/to/your/keyfile nextflow.yaml
```