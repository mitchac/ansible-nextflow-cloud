## goal - configure instance on Nectar / Melbourne Research Cloud

### Step 
Install ansible

### Step 
Clone this repo to your computer

### Step 
Install ansible roles with following command/s
```
ansible-galaxy install geerlingguy.java
ansible-galaxy install andrewrothstein.miniconda
ansible-galaxy install stefangweichinger.rclone
```
### Step
Get the IP address of your cloud instance and edit this in the 'hosts' file. Edit the path to your private ssh key file in the same file. 

### Step
Run the playbook with the following command:
```
ansible-playbook -i hosts nextflow.yaml
```