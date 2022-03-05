
First you need create in your pc, database with name: school

`CREATE DATABASE school`;

After you need create a table: students

`USE school`;

``` 
CREATE TABLE students(id int not null auto_increment ,
                      name varchar(200) not null, 
                      mobile varchar(200) not null, 
                      course varchar(200) not null,
                      primary key (id)
                     );
```

and now you need modify 3 variables in Reg.java file to working correctly

line 28: dbPathName = ""; 
line 29: dbUser = "";
line 30: dbPasswd = "";


dbPathname           = set here your database path: jdbc:mysql://[path]/school

dbuser && dbPasswd   = user and password in your Mysql
