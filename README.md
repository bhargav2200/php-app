# php-app
sample php application to use with AWS RDS to check how the data is being stored in the database

**prerequisite**
   ```
   yum install mysql -y
   yum install mysql-libs -y
   yum install php-mysql -y
   ```

In ram.php update below values with actual values

```
$servername = "ramdb.cbbcw13tzpvs.eu-west-2.rds.amazonaws.com";  RDS endpoint 
$username = "ramdb";  # Database username 
$password = "*****"; # Database password
$dbname = "ramdb"; #Database name to insert data
```
prior to this we need to create a table Persons with below mysql command

```

CREATE TABLE Persons (
    id int,
    lastname  varchar(255),
    firstname varchar(255),
    address varchar(255),
    city varchar(255)
);
```
