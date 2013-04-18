---
layout: post
title: "Just a reminder: mysql commands"
date: 2013-04-18 10:45
comments: true
categories:
 - mysql 
---

Create a database:
```mysql
CREATE DATABASE database_name;
```

Create a mysql user:
```mysql
CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';
```

Give permissions to a user:
```mysql
GRANT ALL PRIVILEGES ON database_name.* TO 'username'@'localhost';
```
Reload permisions
```mysql
FLUSH PRIVILEGES;
```
