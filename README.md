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
### Step
Access your cloud computer 
```
ssh -i path/to/pem/file remote@IP
```

### Step
Change nextflow owner and permissions
```
sudo chown ubuntu /usr/local/bin/nextflow
sudo chmod 755 /usr/local/bin/nextflow
```
