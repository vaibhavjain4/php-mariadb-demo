# PHP-MariaDB-Demo
## Prepare Database <br/> </br>
### Create a mariadb database :<br>
Database Name : studentdb
<br> <br>
### Create a table students using following sql : <br>
Create table students (student_id int(2), first_name varchar(30), last_name varchar(30), hrs_completed int(3), hrs_attempted int(3), gpa_points int(2), major varchar(50), advisor_id int(5), email varchar(256));
<br>
<br> <br>
### Insert a value using sql : <br>
Insert into students values (1, 'Vaibhav', 'Jain', 10, 8, 9, 'Science', 231, 'student@email.com'); 
<br><br> <br>
### Create a table advisors using following sql : <br>
Create table advisors (advisor_id int(3), name varchar(256), email varchar(256)); 
<br><br> <br>
### Insert a value using sql : <br>
Insert into advisors values (231, ‘Mr. Advisor’, ‘advisor1@email.com’);
<br><br>
#### IMPORTANT NOTE : Advisor ID needs to match in both tables otherwise record display and insertion will fail through app user interface. Insert as many values are required.
<br/> <br/>
## Update DB Connection String Values in getStudentData.php
$dsn = "mysql:host=172.30.37.79; port=3306 ;dbname=studentdb; charset=utf8"; <br>
$username = "dbadmin"; <br>
$password = "dbpassword"; <br>

## Build PHP S2I using git repo url
