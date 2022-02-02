# final_project

##How to run:
Run this command in terminal
```
mkdir -p ./dags ./logs ./plugins
```
```
echo -e "AIRFLOW_UID=$(id -u)" > .env
```
```
docker-compose up airflow-init
```
```
docker-compose up
```
Copy and paste all the contents of the `Scripts` folder to the `/dags` folder 
