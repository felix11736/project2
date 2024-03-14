# project2 create data warehouse


kelompok 2 Data Crafters 

tech stack:
python 3.12.o 
(env,dbt loacalhost 8080)


dbeaver 


postgress sql 



![nvoids](https://github.com/felix11736/project2/assets/111951543/4ffa4b13-bc3b-4b46-a27d-d820715c53bc)




============ WINDOWS ===================
Create your project directory
Run pip install virtualenv in Shell CMD
In Shell run cd my-project
Run virtualenv --python C:\Path\To\Python\python.exe env
Activate .\env\Scripts\activate
Install DBT pip install dbt-core==1.6.0 dbt-postgres==1.6.0
============ DBT Setup Part ============
Change your terminal directory to your project directory
Initialize DBT project dbt init
To validate connection change directory to the root project and run dbt debug
Run your first model dbt run -s my_first_dbt_model
If database not found don't forget to create it first using CREATE DATABASE <DB_NAME>;
Setup profiles.yml https://docs.getdbt.com/docs/core/connect-data-platform/snowflake-setup
Setup sources https://docs.getdbt.com/docs/build/sources
Once the model was ran open dbt UI dbt docs generate then run dbt docs serve
=========== BUILD DATA WAREHOUSE ============
Change directory to dbt_project
Create intermediete directory inside models directory:
Create dim_customer.sql
Create dim_time.sql
Create dim_product.sql
Create fact_sales.sql
Create mart directory inside models directory:
Create mart_revenue_monthly.sql
Run this command in the terminal to build model dbt run
Run this command to generate DBT documentation dbt docs generate
Run this command to generate DBT UI dbt docs serve --port 8080




