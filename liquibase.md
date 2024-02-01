## liquibase
- one changelog per release with changesets

liquibase --driver=org.postgresql.Driver \
  --classpath=myFiles/postgresql-9.4.1212.jre7.jar \
  --changeLogFile=myFiles/db.changelog-1.0.xml \
  --url="jdbc:postgresql://localhost:5432/recipes" \
  --username=postgres \
  --password=postgres \
  generateChangeLog