# final_project

How to run:

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
Copy and paste all the contents of the `scripts` folder to `dags` folder 

The folder structure will look like this: 

![Capture](https://user-images.githubusercontent.com/89019518/152134533-3836f03a-43ea-445f-ad7c-a30f4a98ce00.PNG)
