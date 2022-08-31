
# WEB STACK IMPLEMENTATION (LEMP STACK)
## STEP 1 – INSTALLING THE NGINX WEB SERVER
In order to display web pages to our site visitors, we are going to employ Nginx, a high-performance web server. We’ll use the apt package manager to install this package.

Since this is our first time using apt for this session, start off by updating your server’s package index. Following that, you can use apt install to get Nginx installed:
![Install ngix](https://user-images.githubusercontent.com/110794738/187564484-59c60ffd-63e3-4cc5-b11c-22ee1fb1b262.PNG)

![welcome to ngix](https://user-images.githubusercontent.com/110794738/187564655-f82d3a08-63ef-4b70-a4d1-b2ee78e2c760.PNG)

## STEP 2 — INSTALLING MYSQL
Now that you have a web server up and running, you need to install a Database Management System (DBMS) to be able to store and manage data for your site in a relational database. MySQL is a popular relational database management system used within PHP environments, so we will use it in our project.

![Installing Mysql](https://user-images.githubusercontent.com/110794738/187564904-1f75a553-afca-4350-9572-91708a59c28a.PNG)

## STEP 3 – INSTALLING PHP

![installing php](https://user-images.githubusercontent.com/110794738/187565503-491decc1-af4f-4d60-be67-7df8371c860a.PNG)

## STEP 4 — CONFIGURING NGINX TO USE PHP PROCESSOR
When using the Nginx web server, we can create server blocks (similar to virtual hosts in Apache) to encapsulate configuration details and host more than one domain on a single server. In this guide, we will use projectLEMP as an example domain name.

On Ubuntu 20.04, Nginx has one server block enabled by default and is configured to serve documents out of a directory at /var/www/html. While this works well for a single site, it can become difficult to manage if you are hosting multiple sites. Instead of modifying /var/www/html, we’ll create a directory structure within /var/www for the your_domain website, leaving /var/www/html in place as the default directory to be served if a client request does not match any other sites.
![php nglx](https://user-images.githubusercontent.com/110794738/187565945-baa229d5-ab98-4bf7-9411-18375cc37c56.PNG)

![ngx-php-processor](https://user-images.githubusercontent.com/110794738/187566251-2d136c64-00be-452c-b6cf-70036fd03898.PNG)

## STEP 5 – TESTING PHP WITH NGINX

![testing_php_nglx](https://user-images.githubusercontent.com/110794738/187566590-2235bd52-7f30-411c-bf8b-44c1711e8825.PNG)

## STEP 6 – RETRIEVING DATA FROM MYSQL DATABASE WITH PHP (CONTINUED)
In this step you will create a test database (DB) with simple "To do list" and configure access to it, so the Nginx website would be able to query data from the DB and display it.

We will create a database named example_database and a user named example_user, but you can replace these names with different values.
First, connect to the MySQL console using the root account

![todo_list](https://user-images.githubusercontent.com/110794738/187567161-6c00510c-3bbe-4d17-a094-91f452494cf8.PNG)


