# hi  :wave:


First you need to create database with name: school

`CREATE DATABASE school;`

After that you need to create the table: students

`USE school;`

``` 
CREATE TABLE students(id int not null auto_increment ,
                      name varchar(200) not null, 
                      mobile varchar(200) not null, 
                      course varchar(200) not null,
                      primary key (id)
                     );
```

and now you need to modify 3 variables in Reg.java file to working correctly:

```
line 28: dbPathName = "";  // set here your database path like: jdbc:mysql://[path]/school  
line 29: dbUser = "";      // your user in mysql  
line 30: dbPasswd = "";    // your password in mysql  
```

