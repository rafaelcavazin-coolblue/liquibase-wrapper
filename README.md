### Steps:

- must have java installed.
- brew install maven
- need to install the driver manually (it's on ./lib)
```
mvn install:install-file -Dfile=sqljdbc4-4.0.2206.100.jar -DgroupId=com.microsoft.sqlserver\ 
-DartifactId=sqljdbc4 -Dversion=4.0.2206.100 -Dpackaging=jar
```

- adjust liquidbase properties
- adjust change-log.xml
- run maven install

```
mvn clean install
```

-run a liquibase cmd or any other [Docs](http://www.liquibase.org/documentation/maven/)

```
mvn liquibase:update
```