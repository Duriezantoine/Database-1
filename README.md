# Database-1
ysql> INSERT INTO school (name, country, capacity) VALUES ('Beauxbatons Academy og magic',' FRANCE' , 550);
Query OK, 1 row affected (0.09 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('Castelobruxo',' Brazil' , 380);
Query OK, 1 row affected (0.12 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('DURMSTRANG Institute',' Norway' , 570);
Query OK, 1 row affected (0.11 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('HOgwarts Shcool of
Witchraft and Wizardry',' United Kingdom' , 450);
Query OK, 1 row affected (0.10 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('Livermony School of WItchraft and Wizardry',' USA' , 300);
Query OK, 1 row affected (0.13 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('Koldovstoretz',' Japan' , 800);
Query OK, 1 row affected (0.16 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('Mahoutokoro School
of Magic',' Japan' , 800);
^[[AQuery OK, 1 row affected (1.41 sec)

mysql> INSERT INTO school (name, country, capacity) VALUES ('Uagadou School of Magic',' Uganda' , 350);
Query OK, 1 row affected (0.10 sec)

mysql> UPDATE school 
    -> SET country = 'Sweden' 
    -> WHERE name = 'Durmstrang Institute';
Query OK, 1 row affected (0.08 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> PDATE school 
    -> SET capacity = 700 
    -> WHERE name = 'Mahoutokoro School of Magic';
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'PDATE school 
SET capacity = 700 
WHERE name = 'Mahoutokoro School of Magic'' at line 1
mysql> PDATE school  SET capacity = 700  WHERE name = 'Mahoutokoro School of Mag
ic';UPDATE school 
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'PDATE school  SET capacity = 700  WHERE name = 'Mahoutokoro School of Magic'' at line 1
    -> SET capacity = 700 
    -> WHERE name = 'Mahoutokoro School of Magic';
Query OK, 1 row affected (0.12 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> DELETE from school 
    -> WHERE name LIKE '%Magic%';
Query OK, 3 rows affected (0.14 sec)

mysql> mysql> SELECT * from school;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> SELECT * from school' at line 1
mysql> SELECT * from school;
+----+--------------------------------------------+-----------------+----------+
| id | name                                       | country         | capacity |
+----+--------------------------------------------+-----------------+----------+
|  2 | Castelobruxo                               |  Brazil         |      380 |
|  3 | DURMSTRANG Institute                       | Sweden          |      570 |
|  4 | HOgwarts Shcool of Witchraft and Wizardry  |  United Kingdom |      450 |
|  5 | Livermony School of WItchraft and Wizardry |  USA            |      300 |
|  6 | Koldovstoretz                              |  Japan          |      800 |
+----+--------------------------------------------+-----------------+----------+
5 rows in set (0.00 sec)

mysql> 

