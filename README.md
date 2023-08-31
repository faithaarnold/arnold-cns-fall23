# 1/c Faith Arnold - CNS Homework #1 - 30 August 2023 
## Provisioning a Virtual Machine
To provision a web server on Vagrant, I first created an html file for the web page I wanted to display
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/dbe55652-3f6c-4e4d-9af6-3351e5ae1fb6)
Then, the provisioning script that allowed Vagrant to download Apache to link the files directory and the location of content you want to provision.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/d1a55e9c-cfce-47a4-b736-a7d15a9eff46)
For these changes to work in the Vagrant environment, a "config.vm.provision" line needs to be added to the Vagrantfile along with the file path of the provision script.
After these changes, ssh into Vagrant and use a "wget" command to display the html.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/900c0b33-84ce-47c7-8d3e-ebf6df36002f)

## Configure the Network
This tutorial allowed access to the guest machine from the host machine. To do this, I added the "config.vm.network :forwarded_port, guest: 80, host: 4567" command to my Vagrantfile. After doing this, the html file I created was able to be accessed through http://127.0.0.1:4567/ 
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/97013fd1-961f-44a3-9593-ddeddae1a525)

##Shell Provisioner
The Vagrant Shell provisioner is a great method for users new to Vagrant to upload and run script in the guest machine. Shell executes scripts using ssh, making it much simpler to use in comparison to full configuration management systems.
