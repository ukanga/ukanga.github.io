---
layout: post
title: "some lessons on altering mysql storage engine"
date: 2013-05-20 11:46
comments: true
categories: 
- mysql
- innodb
- MyISAM
---

Check what storage engine a particular table is using:
```mysql
SELECT table_name, engine FROM INFORMATION_SCHEMA.TABLES;
```

Changing storage engine of a table;
```mysql
ALTER TABLE `table_name1` ENGINE = MyISAM;
```

When altering a table engine from InnoDB to MyISAM, you have to delete all constraints
 on the table otherwise you will get a foreign key constraint error. You can check the
 constraints within a form using
```mysql
SHOW CREATE TABLE `table_name1`;
```
You can then drop the constraints like:
```mysql
ALTER TABLE `table_mame1` DROP FOREIGN KEY `user_id_refs_id_1e020b58278eec2b`;
````
