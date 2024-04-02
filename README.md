# Neo4j Movies Repository

## Docker Compose

This project uses docker compose. Docker Compose is a tool for defining and running multi-container applications.

To launch this web application, you can run the following command, from the root folder of the project.

```
git clone git@github.com:Eliie58/neo4j_movies_repository.git
cd neo4j_movies_repository
docker compose up -d --build
```

### Database

The neo4j database is accesible from [http://localhost:7474/browser/](http://localhost:7474/browser/)

### Web Application

The web application, deployed using [Streamlit](https://streamlit.io/) is accesible from [http://localhost:8080](http://localhost:8080)

## Data Loading

Data used is available under the [data](./data/) folder.

To load the data into the database, you can use the following commands:

```
LOAD CSV WITH HEADERS FROM 'file:///actors.csv' AS row
...
```
