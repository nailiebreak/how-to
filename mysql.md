# Basic Commands

## _Q1. How to restart MySQL_

`sudo systemctl restart mysql.service`

## _Q2. How to check whether the MySQL server is running_

`sudo netstat -tap | grep mysql`

## _Q3. Create a database with given charset_

`CREATE DATABASE mydatabase CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci;`

## [_Q4. Create a user_](https://dev.mysql.com/doc/refman/8.0/en/grant.html#grant-overview)

`CREATE USER 'user'@'localhost' IDENTIFIED BY 'password'`

`GRANT ALL ON *.* TO 'user'@'localhost'`

# Errors

## [_Q1. Error: Access denied for user 'root'@'localhost'_](https://dev.mysql.com/doc/refman/8.0/en/resetting-permissions.html)

> Ubuntu

1. Add `skip-grant-tables` under `[mysqld]` in **_/etc/my.cnf_**.
   ```yaml
   [mysqld]
   skip-grant-tables
   ```
2. Restart MySQL and execute following statements.
   ```yaml
   $ mysql -u root
   $mysql> use mysql;
   $mysql> FLUSH PRIVILEGES;
   $mysql> UPDATE USER SET authentication_string=password('new_password') WHERE user='root';
   ```
3. Comment `skip-grant-tables` and restart MySQL with `mysql -u root -p`.

> MacOS

1. Restart MYSQL and execute following statement.

```shell
brew services stop mysql
mysql.server start --skip-grant-tables

$ mysql -u root
$mysql> UNINSTALL COMPONENT 'file://component_validate_password';
mysql> ALTER USER 'root'@'localhost' IDENTIFIED BY 'new_password';
```

2. Restart MYSQL by using `brew services start mysql`

## _Q2. Error: Plugin 'unix_socket' is not loaded_

```yaml
$ mysql -u root -p
$mysql> use mysql;
$mysql> UPDATE USER SET plugin='mysql_native_password' WHERE user='root';
```
