# Airflow solution

### install necessary packages
1. install [Docker](https://docs.docker.com/engine/installation/)
2. install [docker-compose](https://docs.docker.com/compose/install/) >= v1.27.0

### Run docker-compose
3. Create airflow backend DB:  `docker-compose up airflow-init`
4. run airflow: `docker-compose up`

### Enter UI
The webserver available at: http://localhost:8080. The default account has the login: <br>
user `airflow` <br>
password `airflow`

### DAG
At the moment there is one example pipeline in teh dags/ folder:
```
.
├── dags
│   └── example.py

```

