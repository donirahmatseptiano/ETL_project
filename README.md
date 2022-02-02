# Description

This project is about Dockerize ETL Pipeline using ETL tools Airflow that extract Public API data from PIKOBAR (for area Jawa Barat province), then load into MySQL (Staging Area) and finally aggregate the data and save into PostgreSQL.

API Specification:

![image](https://user-images.githubusercontent.com/89019518/152145063-b3904bee-94da-4b4c-a589-91e0c02331c5.png)

API Request Example:

```curl -X GET "https://covid19-public.digitalservice.id/api/v1/rekapitulasi_v2/jabar/harian?level=kab" -H "accept: application/json"```

API response example:

![image](https://user-images.githubusercontent.com/89019518/152144976-19b7863f-cb18-49f7-859a-63445d10ad86.png)

# How to run:

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
