#### orbuildwebappflaskneo4
#####Neo4j
######install
set:options->server configuration,set
```
dbms.security.auth_enabled=false
```
basic cypher:
```
MATCH (p:Person)-[:ACTED_IN]->(m:Movie) RETURN p.name AS person, m.title AS title LIMIT 1
```

#####Project setup
######virtualenv
```
mkdir Virtualenvs
cd Virtualenvs
virtualenv orbuildwebappflaskneo4
source orbuildwebappflaskneo4/bin/activate
```
```
pip install py2neo
```
