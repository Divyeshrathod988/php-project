# php-project

#install all packages
when used ubantu server.
1.apt install php php mysql-server
2.apt install apache2
3.apt install php-mysqli


=> mysql -h database-1.cp6mokg8yl9d.ap-south-1.rds.amazonaws.com -u root  -p
used your id password and endpoits
1. CREATE database php_employee_management;
2.USE php_employee_management;
3.CREATE TABLE employee (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  
  email VARCHAR(100) NOT NULL,
  address TEXT NOT NULL
);

4 . ALTER TABLE employee
ADD COLUMN phone VARCHAR(20) NULL,
ADD COLUMN created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP;


=> you can add  phone colum cteare table time 

5 show tables;


CREATE TABLE emloyee (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    subject VARCHAR(150) DEFAULT 'No Subject',
    message TEXT DEFAULT 'No Message',
    website VARCHAR(200),
    gender ENUM('Male', 'Female', 'Other') NOT NULL,
    submitted_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
