# Miles-pbl
DAREY.IO Projects

# WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS
What is a Technology stack?
A technology stack is a set of frameworks and tools used to develop a software product. This set of frameworks and tools are very specifically chosen to work together in creating a well-functioning software.

## Connecting to EC2 Instance Using Ubuntu server


![Instance](https://user-images.githubusercontent.com/110794738/186622675-83ffcf0c-6752-4cde-af1b-3d8a94fe08f8.PNG)

INSTALLING APACHE AND UPDATING THE FIREWALL

sudo apt update

![Sudo apt update](https://user-images.githubusercontent.com/110794738/186624207-522373ab-9d1e-49b0-9d6f-7c8e3c0e30db.PNG)

sudo systemctl status apache2

![Sudo syeteml](https://user-images.githubusercontent.com/110794738/186627583-3059847a-3f34-4984-aa45-ec5179a054f9.PNG)

Web server is now correctly installed and accessible through firewall.

![apache2 default](https://user-images.githubusercontent.com/110794738/186630343-8c04b3c5-faa2-41d3-93f4-010ca0751eff.PNG)

INSTALLING MYSQL

![Installing Mysql](https://user-images.githubusercontent.com/110794738/186632580-e39fe8cd-72a3-4c94-8071-7106205bc4a9.PNG)

![mysql](https://user-images.githubusercontent.com/110794738/186636702-f8dc1e99-6cd3-4a7f-affd-2cb02b831e47.PNG)

sudo mysql_secure_installation

![mysql2](https://user-images.githubusercontent.com/110794738/186641104-2e2978f1-fd05-4655-9a02-b31dfb4c2385.PNG)

## INSTALLING PHP

sudo apt install php libapache2-mod-php php-mysql

![installing php](https://user-images.githubusercontent.com/110794738/186643412-d71ab59d-363d-4b03-9ea4-afff75d4fdb1.PNG)

Command to run php

php -v

![php](https://user-images.githubusercontent.com/110794738/186644515-50b83632-f791-4f0a-9272-f3bb533dfc68.PNG)

 CREATING A VIRTUAL HOST FOR YOUR WEBSITE USING APACHE
 
 sudo mkdir /var/www/projectlamp
![mkdir](https://user-images.githubusercontent.com/110794738/186702188-4fe2083c-e740-4e51-ac89-3799343fa9e9.PNG)

![ip](https://user-images.githubusercontent.com/110794738/186702808-f30b7e25-cbf6-4731-b2d0-8dd25e85d2e2.PNG)

ENABLE PHP ON THE WEBSITE

Create a new file named index.php inside your custom web root folder

vim /var/www/projectlamp/index.php

This will open a blank file. Add the following text, which is valid PHP code, inside the file:

<?php
phpinfo();

![phpv](https://user-images.githubusercontent.com/110794738/186710091-854c078f-5f0a-462c-8e98-85e79d20073e.PNG)

<?php
phpinfo();

![phpv](https://user-images.githubusercontent.com/110794738/186711580-c4ed2696-4ee6-4c13-86fa-552660050979.PNG)

