Section #1 - Purpose of PHP Crude CRUD Application:
  The PHP Crude CRUD application is a simple PHP based web application that allows users to perform CRUD operations (Create, Read, Update, Delete) in a database such as mySQL. IT provides a basic user unterface for managing database records without having to write any SQL code.
  
Section #2 - Overview of creating an entirely new application architecture and stack:
  To create a new applicatoin architecture and stack from the ground up, the following steps can be followed:
    1. Provision a new virtual machine (VM) with the suggested configuration.
    2. Go to Ubuntu website and install the Ubuntu 20.04 operating system file.
    3. Install Apache 2 and PHP.
    4. Configure the connection and credentials needed for PHP to connect to the database.
    5. Deploy the PHP crude CRUD application.
    
 Section #3 - Suggested Virtual Machine Configuration:
    Disk: 20 GB 
    CPU: 2 cores
    RAM: 4 GB
    
 Section #4 - Creating VirtualBox Virtual Machine:
    1. Download and install VirtualBox
    2. Click on the "new" button to create a new VM
    3. Set the RAM size, CPU cores, and storage size
    4. Fill in remaining feilds according to preference information
    5. Click "create" to create new VM
     
  Section #5 - Installing Ubuntu 20.04 Operating System:
    1. Download Ubuntu 20.04 ISO file.
    2. Start the VirtualBox VM and use the Ubuntu 20.04 ISO
    3. Follow instructions to install
    
   Section #6 - Installing Apache 2 and PHP:
      1. SSH into VM from terminal using ip address and login information
      2. Run the command sudo apt-get update
      3. Install Apache 2 by running the command: sudo apt-get installe apache2
      4. Install PHP by running the command: sudo apt-get install php libapache2-mod-php php-mysql
     
   Section #7 - Installing MySQL:
      1. Install mySQL by running the command: sudo apt-get install mysql-server
      2. during installation, set a root password for mySQL
      
   Section #8 - Configuring PHP and mySQL connection:
      1. Open the PHP configuration file located at /etc/php/7.x/apache2/php.ini
      2. Uncomment the following line: ;extention=mysqli
      3. Restart apache by running the command: sudo systemctl restart apache2
      4. Create a new MYSQL user with the necessary privileges: CREATE USER 'phpcrud'@"localhost' IDENTIFIED BY 'password'; CRANT ALL PRIVELGES ON * . * TO 'phpcrud'@localhost';
      5. Update the PHP code with the database connection information
      
   Section #9 - Deploying PHP crude CRUD application:
      1. Download the PHP Crude CRUDE application code.
      2. Copy the code to the Apache web root directory
      3. Import the database into the PHP file
      4. Access the application by opening a web browser and entering the servers IP address or domain name.
      
   Section #10 - Suggested System Tests:
      1. Verify that the PHP crude CRUD application can perform CRUD operations the database.
      2.Test the application's security by attempting SQL injection attacks.
      3.Test the application's performance by simulating multiple user requests at once.
      
    
    
