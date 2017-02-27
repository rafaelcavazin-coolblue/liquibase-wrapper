### Steps:

- must have java installed.
- brew install maven
- need to install the driver manually (it's on ./lib)
```
make
```
- adjust liquidbase properties
- adjust selena.changelog-master.xml
- add your changes
- run maven install

```
mvn clean install
```

-run a liquibase cmd or any other [Docs](http://www.liquibase.org/documentation/maven/)

```
mvn liquibase:update -Denvironment=(development/uat/prod)
```
