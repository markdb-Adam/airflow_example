# Airflow solution

### install necessary packages
1. install [Docker](https://docs.docker.com/engine/installation/)
2. install [docker-compose](https://docs.docker.com/compose/install/) >= v1.27.0

### Add requirements
3. Build custom airflow image with requirements <br>
`docker build . -f Dockerfile --tag airflow_and_requ:0.0.1`


### Run docker-compose
4. Create airflow backend DB:  `docker-compose up airflow-init`
5. run airflow: `docker-compose up`

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

