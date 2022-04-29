# project-2
my-sql
![webserver9](https://user-images.githubusercontent.com/29538033/165902412-0769c7b0-c4d4-430a-a764-2985589a4cd4.PNG)
![webserver9 PNG1](https://user-images.githubusercontent.com/29538033/165902569-9e66f8f0-b154-4124-b2e6-2f7b4ca76996.PNG)
..............................................................................................................................
now created ubuntu machine in aws with http and sql port open
![webserver9 1](https://user-images.githubusercontent.com/29538033/165903124-a4255189-816e-49b7-99f7-6b480b82ce91.PNG)
Now install my -sql on ubuntu server
installation steps
....sudo apt update
....sudo apt install mysql-server
....sudo systemctl start mysql.service
now configure mysql 
....sudo mysql_secure_installation
after the command is run provide the password
![Capture](https://user-images.githubusercontent.com/29538033/165904871-2ed1ce11-0698-4dac-8c08-119eb5679b60.PNG)
NOW Creating a Dedicated MySQL User and Granting Privileges
....sudo mysql
![Capture2](https://user-images.githubusercontent.com/29538033/165906379-6b23ff1f-0b46-4bcf-b375-7f00ba33e40b.PNG)
NOW CREATE a user with full previlages
... CREATE USER 'myuser'@'localhost' IDENTIFIED BY 'MYPASS';
... CREATE USER 'myuser'@'%' IDENTIFIED BY 'mypass';
now give full previliages
...GRANT ALL ON *.* TO 'myuser'@'localhost';
...GRANT ALL ON *.* TO 'myuser'@'%';
...FLUSH PRIVILEGES;
