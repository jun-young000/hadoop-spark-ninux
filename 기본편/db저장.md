예시

```
REATE DATABASE customer_db;
USE customer_db;

CREATE TABLE GURA (
    no INT UNSIGNED NOT NULL AUTO_INCREMENT,
    name CHAR(20) NOT NULL,
    age TINYINT,
    phone VARCHAR(20),
    email VARCHAR(30) NOT NULL,
    address VARCHAR(50)
	);
```

ERROR 3948 (42000): Loading local data is disabled; this must be enabled on both the client and server sides  

해결방법

mysql> show global variables like 'local_infile';



입력하면
+---------------+-------+
| Variable_name | Value |
+---------------+-------+
| local_infile  |  OFF  |
+---------------+-------+



mysql> set global local_infile=true;
이걸 입력하면 OFF 가  ON으로 바뀐다

mysql> exit
mysql --local_infile -u root -p





```
CREATE TABLE ONEGIRL(
    ID  INT,
    DATE _CODE INT,
    LOCAL_CODE INT,
    TOTAL INT,
    UNDER_20 INT,
    20_24 INT,
    25-29 INT,
​	30_34 INT,
​	35_39 INT,
​	40_44 INT,
​	45_49 INT,
​	50_54 INT,
​	55_59 INT,
​	60_64 INT,
​	65_69 INT,
​	70_74 INT,
​	75_79 INT,
​	80_84 INT,
​	OVER_85 INT, 
 	PRIMARY KEY(ID)
);
```

```
LOAD DATA LOCAL INFILE  '/home/data/project/one.csv'

INTO TABLE ONEGIRL

FIELDS TERMINATED BY  ',';
```

```
db 저장

LOAD DATA INFILE `파일경로/파일이름.csv` 

INTO TABLE 테이블이름 

FIELDS TERMINATED BY `,`;
```



```
CREATE TABLE PROPORTION(
    ID  INT,
    DATE _CODE INT,
    LOCAL_CODE INT,
    PROPROTION INT,
    MEN_POPULATION INT,
 	WOMAN_POPULATION INT,
 	PRIMARY KEY(ID)
 );
```

```
LOAD DATA LOCAL INFILE  '/home/data/project/nokor.csv'

INTO TABLE ONEGIRL

FIELDS TERMINATED BY  ',';
```

```

```

```
CREATE TABLE safety(
    ID  INT,
    LOCAL_CODE INT,
	ADDR STR,
	PRIMARY KEY(ID)
 );
```

```
LOAD DATA LOCAL INFILE  '/home/data/project/gurde.csv'

INTO TABLE ONEGIRL

FIELDS TERMINATED BY  ',';
```

---------------------------

```

```

```
LOAD DATA LOCAL INFILE  '/home/data/project/nokor.csv'

INTO TABLE ONEGIRL

FIELDS TERMINATED BY  ',';
```

