# Sample Spark Java

A simple working example of Spark with Java

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