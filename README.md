# Sample Spark Java

A simple working example of Spark with Java.

## Tutorial
- [MySQL table to JSON with 10 lines of Spark
](https://www.geekyhacker.com/2020/04/21/mysql-table-to-json-with-10-lines-of-spark/)

## How to run

### Bring up docker and create table

```bash
$ docker-compose up -d
$ ./db_initializer.sh
```

### Compile and run with Maven

```bash
$ cd .. && mvn clean compile exec:java
```

First 3 million records test rows inserted to the database. Then Sparks read those records and convert them to JSON 
in `books_json` directory. 
