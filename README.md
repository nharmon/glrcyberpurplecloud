# glrcyberpurplecloud
Provisioning notes for PurpleCloud

## Windows VM

Powershell

> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

Go to Windows Store, and install 


## Inside WSL

> sudo apt install python3 python3-pip azure-cli

> wget -O- https://apt.releases.hashicorp.com/gpg | gpg --dearmor | sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg
> echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
> sudo apt update && sudo apt install terraform

> pip install faker

> git clone https://github.com/iknowjason/PurpleCloud

> cd PurpleCloud

> az login

> python3 ad.py --domain_controller --ad_domain MrRobot.local --admin GLRadmin --password Cyber2022! --ad_users 50 --endpoints 3 --location eastus --domain_join --helk 
--resource_group First-Lastname

> terraform init

> terraform plan -out out.plan

> terraform apply out.plan
