# banking site
Banking Application

This is a simple banking application that allows users to register, login, and perform transactions. It is built using Node.js, Express, and MySQL.
Installation


Step 1: Visit the MySql Website
Open your browser and go to the MySql website: https://www.mysql.com/.
Go to the Download link on the top of the navigation bar 

Step 2: Pick MySql Community Edition
On the MySql Download page, find the section labeled Mysql Community (GLP) Downloads 
Click on the MySql Community Server link.

Step 3: Choose your operating system
On the MySql Community server downloads page, you’ll see a drop-down menu to select your operating system
Choose your operating system 
Windows 
Mac 
Linux

Step 4: Download the installer
Windows:
After selecting "Microsoft Windows," you'll be taken to the download page.
Choose the appropriate installer version. Generally, you should select the "Windows (x86, 64-bit), MSI Installer" for most systems.
Click on the "Download" button next to the MSI installer.
You may be prompted to log in or sign up for an Oracle Web account. You can either log in, sign up, or click on "No thanks, just start my download" to download without logging in.
MacOS:
After selecting "macOS," you'll be taken to the download page.
Choose the "macOS 10.15 (x86, 64-bit), DMG Archive" or the version that matches your macOS version.
Click on the "Download" button next to the DMG installer.
You may be prompted to log in or sign up for an Oracle Web account. You can either log in, sign up, or click on "No thanks, just start my download" to download without logging in.
 Linux:
After selecting "Linux," you'll be taken to the download page.
Choose your Linux distribution from the list (e.g., Ubuntu, Red Hat, etc.).
Follow the instructions for your specific distribution to download the appropriate package.

Step 5: Run the  the installer
	
Windows 
Locate the MSI installer file and start the installation process 
Follow the installation wizard steps to complete the installation. You will need to configure the MySQL server during this process, including setting a root password

macOS
Locate the downloaded DMG file and start the installation process and double click the .pkg file to start the installation process.
Follow the installation wizard steps to complete the installation. You will need to configure the MySQL server during this process, including setting a root password

Linux 
Open a terminal window.
Use the package manager for your Linux distribution to install MySQL. For example, on Ubuntu, you can use:
sudo apt get update, 								sudo apt install mysql-server
Follow the prompts to complete the installation and configure the MySQL server, including setting a root password.

Step 7: Verify the Installation
Open a command prompt (Windows) or terminal (macOS/Linux).
Run the following command to verify that MySQL is installed correctly and running
Mysql –version

Step 8: Start MySql server 
Windows
MySQL server should start automatically after installation. If not, you can start it manually from the Windows Services Manager.
Open the Services Manager, find MySQL in the list, and click Start
MacOS
MySQL server should start automatically after installation. If not, you can start it manually from the Windows Services Manager.
Open the Services Manager, find MySQL in the list, and click Start
Linux
Use the following command to start the MySQL server:
sudo mysql_secure_installation
Run the MySQL secure installation script to enhance security:
sudo mysql_secure_installation
Follow the prompts to set up the root password, remove anonymous users, disallow root login remotely, remove test databases, and reload privilege tables.

Step 9: Access MySql
In terminal or command prompt login to mysql as root user or another user with the same privileges 
mysql -u root -p
Enter your MySQL root password when prompted.

Step 10: Create new database
 SQL command for creating a database.
CREATE DATABASE user_accounts;(replace user_accout with your desired name for the database.)
Verify that the database was created 
SHOW DATABASES; 

Step 11: Select the database 
SQL command for selecting a database 
USE user_accout(replace user_accout with your desired name for the database)

Step 12: Create a table:
The SQL
CREATE TABLE Users (
id INT AUTO_INCREMENT PRIMARY KEY,
username VARCHAR(50) NOT NULL UNIQUE,
password VARCHAR(255) NOT NULL,
bank_money DECIMAL(10, 2) NOT NULL DEFAULT 0.00
);


Verify the table creation
SHOW TABLES;
 Check the table structure
DESCRIBE users;

Step 13: install NPM 
To download and install npm (Node Package Manager), you need to install Node.js, which includes npm. Here are the steps to do this:
Visit the Node.js website: Go to the Node.js download page.
Download the installer: Choose the version suitable for your operating system (Windows, macOS, or Linux). The LTS (Long Term Support) version is recommended for most users.
Run the installer:
Windows: Run the downloaded .msi file and follow the installation prompts.
macOS: Run the downloaded .pkg file and follow the installation prompts.
Linux: Follow the instructions for your specific distribution. You can find detailed instructions on the Node.js website.
Verify the installation:
Open your terminal or command prompt.
Run node -v to check the installed version of Node.js.
Run npm -v to check the installed version of npm.

Step 14: install node.js 
Visit the Node.js website: Open your web browser and go to the Node.js official website.
Download the installer:
On the Node.js homepage, you'll see two versions available for download: the LTS (Long Term Support) version and the Current version. It's generally recommended to download the LTS version for most users, as it is more stable.
Click on the version that suits your operating system (Windows, macOS, or Linux).
Run the installer:
Windows: After downloading, double-click the .msi installer file and follow the installation prompts. The installer will guide you through the setup process.
macOS: After downloading, double-click the .pkg installer file and follow the installation prompts. The installer will guide you through the setup process.
Linux: Follow the specific instructions for your distribution. You can find detailed installation instructions on the Node.js website or use a package manager.
For example, on Ubuntu, you can install Node.js using the following commands:
 Sudo apt update
Sudo apt install nodejs npm 
Verify the installation:
Open your terminal or command prompt.
Run node -v to check the installed version of Node.js.
Run npm -v to check the installed version of npm.

Step 15: Set up 
Create a directory for your project 
mkdir express-mysql-app
cd express-mysql-app
Make sure that the project files are in this directory 	
Initialize a Node.js project:
npm init -y
Install dependencies:
npm install express body-parser mysql2 path express-session cookie-parser hbs

Step 16: start server
In the project file run the following command:
 node scrip.js
Navigate to local host 
