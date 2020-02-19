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
### Step 3
Get the IP address of your cloud instance and edit this in the 'hosts' file. Edit the path to your private ssh key file in the same file. 

### Step 4 
Run the playbook with the following command:
```
ansible-playbook -i hosts nextflow.yaml
```
### Step 4 
Add conda to your path with following command. You may need to change the path to reflect your conda install location..
```
export PATH=/usr/local/Miniconda3-4.7.12.1-Linux-x86_64/condabin:$PATH
```