# Airflow with Local Executor and Postgres 12.5 DB.


### Before run:

 - Correct variable substitution.
 - Install docker-compose https://docs.docker.com/compose/install/
 - If you haven't changed your docker-cmpose.yml. Make sure you have free default ports.
 - Default used ports: 9432, 8080, 5555, 8793.
 - Create directory for /usr/local/airflow/ 
 

### How to run:

 - git clone https://github.com/JumboTee/airflow-LocalExecutor.git
 - docker-compose -f docker-compose.yml up -d


### After run actions:

 - Add default Postgres DB.
 - Go to localhost:8080/admin/connection/
 - Edit postgres_default Connd_Id.

 ### Default Postgres config:
 - POSTGRES_USER=airflow
 - POSTGRES_PASSWORD=airflow
 - POSTGRES_DB=airflow
 - POSTGRES_PORT=9432