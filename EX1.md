# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY:
```
CREATE TABLE student(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```

### OUTPUT:
![image](https://github.com/NAGINENIROHITH/G2_DBMS/assets/118344049/223500df-3d6d-437f-a168-1a80542a3468)


### 2) Change the above student table by adding another attribute department
### SQL QUERY: 
```
ALTER TABLE student ADD Department char(10);
```
### OUTPUT:
![image](https://github.com/NAGINENIROHITH/G2_DBMS/assets/118344049/1ad110f5-b15f-4c00-b102-fbaf1974c1f1)


### 3) Drop the student table
 
### SQL QUERY: 
```
DROP TABLE student;
```
### OUTPUT:
![image](https://github.com/NAGINENIROHITH/G2_DBMS/assets/118344049/23d7e764-57e2-4afe-9229-3c013c54d12b)


### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE student;
```

### OUTPUT:
![image](https://github.com/NAGINENIROHITH/G2_DBMS/assets/118344049/4ad32b24-cf22-4ed4-8cec-3636ada47df9)



### 5) Rename the student table to mystudent

### SQL QUERY: 
```
ALTER TABLE student RENAME TO mystudent;
```

### OUTPUT:
![image](https://github.com/NAGINENIROHITH/G2_DBMS/assets/118344049/1147eae2-dd27-491f-95e5-8c78a9944962)

### RESULT:
Thus a student database has been created and DDL queries are executed successfully.
