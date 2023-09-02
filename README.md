# Neo4j : First steps with Cypher

This repository holds some simple R code examples and notebooks to interact between R/RStudio and a local Neo4J DBMS.

For everything to work it is assumed a local Neo4J installation either using docker:

```bash
docker pull neo4j:4.3.4
docker run --name neo4j -p7474:7474 -p7687:7687 --env NEO4J_AUTH=neo4j/test -d neo4j:4.3.4
```

When doing this on Windows you may also need to run with following parameters:

```bash
--env NEO4J_dbms_connector_https_advertised__address="localhost:7473"
--env NEO4J_dbms_connector_http_advertised__address="localhost:7474"
--env NEO4J_dbms_connector_bolt_advertised__address="localhost:7687"
```

Or simply downloading and installing a desktop version from [Neo4J official website](https://neo4j.com/download-center/#desktop)
