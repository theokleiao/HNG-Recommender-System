This is Task2  assingned to Machine Learning gruops in the ongoing HNG intership programme. The teams are assighned to build a Recommender System for lucid.blog. It wasrequired that the recommendation system should suggest who to follow and what articles to read for a user.
The lucid.blog  database was provided from where we selected the necessary features needed, perform Exploratory Data Analysis and built  a model for our recommendation

To achieve the above listed objectives, the following steps were carried out:

1. The relevant libraries were imported in the jupyter notebook such as 

import pandas as pd
import mysql.connector
from sqlalchemy import create_engine

2. Loaded the dataset

mydb = mysql.connector.connect(host="remotemysql.com",
                              user="8SawWhnha4",
                              passwd="zFvOBIqbIz",
                              database="8SawWhnha4")

engine = create_engine('mysql+mysqlconnector://8SawWhnha4:zFvOBIqbIz@remotemysql.com/8SawWhnha4')


3. fetched  the tables in the dataset

dbcursor = mydb.cursor()
dbcursor.execute('show tables')
for table in dbcursor:
    print(table)

The above steps were carried out to set the data ready for extensive data exploratory analysis.








