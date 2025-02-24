Not using GitHub? Find me on [LinkedIn](https://www.linkedin.com/in/cuong9/)!
# neo4j

Learning 📺 Neo4j

## Docker

```shell
docker run -p 7474:7474 -p 7687:7687 \
    --env NEO4J_AUTH=neo4j/123456 \
    --volume=$HOME/neo4j/data:/data \
    neo4j
```

**Connect to Neo4j**

![login](./.images/login.png)

**Result**

![login_result](./.images/login_result.png)

## Cheat sheet 💅

### Create model & relationship

```
CREATE (john:Person {name: 'John'})
CREATE (joe:Person {name: 'Joe'})
CREATE (steve:Person {name: 'Steve'})
CREATE (sara:Person {name: 'Sara'})
CREATE (maria:Person {name: 'Maria'})
CREATE (john)-[:FRIEND]->(joe)-[:FRIEND]->(steve)
CREATE (john)-[:FRIEND]->(sara)-[:FRIEND]->(maria)
```

### Find all Person

```
MATCH (p:Person) RETURN p
```

![](./.images/1.png)

### 

## Documents

- [Neo4j clauses](https://neo4j.com/docs/cypher-manual/current/clauses/)
- [The Neo4j Cypher Manual](https://neo4j.com/docs/cypher-manual/current/)
- [Neo4j Cheat Sheet](https://simplecheatsheet.com/tag/neo4j-cheat-sheet/)

## License

MIT © [Cuong Tran](https://github.com/103cuong)
