# Build a Natural Language SQL Agent

### Create DB
https://docs.yugabyte.com/preview/sample-data/chinook/

Introduction to the Chinook database
The Chinook database models a comprehensive digital media store ecosystem, featuring interconnected tables that track artists, albums, media tracks, invoices, and customer information. Here's what makes it unique:

The media catalog contains authentic data sourced directly from an Apple iTunes library
Customer and employee records use carefully crafted fictional data, including Google Maps-verified addresses and properly formatted contact details (phone numbers, fax, email addresses)
The sales data spans a 4-year period and was generated programmatically with randomized but realistic values
Key characteristics of the database:

Comprehensive structure with 11 distinct tables
Robust data integrity through indexes and primary/foreign key relationships
Rich dataset containing more than 15,000 records
Below you'll find the entity relationship diagram (ERD) that illustrates how the different components of the Chinook database connect and interact with each other.

![er](er_dia.png)

### Create venv
```bash
pip install virtualenv 
virtualenv my_env # create a virtual environment named my_env
source my_env/bin/activate # activate my_env
```

### Install lib

```bash
python3.11 -m pip install ibm-watsonx-ai==1.0.4 \
ibm-watson-machine-learning==1.0.357 \
langchain==0.2.1 \
langchain-ibm==0.1.7 \
langchain-experimental==0.0.59 \
mysql-connector-python==8.4.0
````

### Connect with MySQL

```bash
create
```

```bash
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Mauh_UvY4eK2SkcHj_b8Tw/chinook-mysql.sql
```

```bash
SOURCE chinook-mysql.sql;
```


