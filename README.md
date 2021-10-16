# incubyte_assessment

## Overview:
This repository made to demonstrate implementation of given [assessment](https://github.com/kaus988/incubyte_assessment/blob/main/Data%20Engineer%20Assignment%20-%20C-DAC.pdf).Also, a dummy database has been created to demonstarte a simple data flow in different formats from server to the local system, using country-based row filteration. For demonstrating working of data pipeline different tools are used which are listed below.
**Concepts:**
- Data processing
- ETL

**Tools & Technologies:**
- Python 
- MySQL Workbench
- Visual Studio Code
- Spyder
- [Pandas](https://pandas.pydata.org/docs/)
- [MySQL connector](https://dev.mysql.com/doc/connector-python/en/connector-python-introduction.html)

## Working:
- Firstly MySQL database has been created with specified schema.
- [```Data_Separation.py```](https://github.com/kaus988/incubyte_assessment/blob/main/programs/Data_Separation.py) python script, fetches database by establishing connection with MySQL server.
- The retrieved data is fitted into pandas dataframe for further table manipulation.
- ```get_data()``` & ```store_file()``` functions are called to fetch the desired data rows and generating ```.csv``` and ```string``` file formats to specified path, accepting country names as parameters for filtering rows. 
- For example: ```store_file("IND")``` generates [```IND.csv```](https://github.com/kaus988/incubyte_assessment/blob/main/outputs/IND.csv) to the specified local path. [click here](https://github.com/kaus988/incubyte_assessment/tree/main/outputs) to see sample output files.

Installation Guide:
- To install ```mysql.connector```:
```
pip install mysql.connector
```
- To install pandas:
```
pip install pandas
```
## References:
- [MySQL Connector Python](https://dev.mysql.com/doc/connector-python/en/connector-python-introduction.html)
- [Pandas docs](https://pandas.pydata.org/docs/)

## Screenshots:

#### Mysql_Workbench_console:
![alt tag](https://github.com/kaus988/incubyte_assessment/blob/main/Screenshots/Mysql_Workbench_Screenshot%202021-10-16%20163902.png)

#### Spyder_console:
![alt tag](https://github.com/kaus988/incubyte_assessment/blob/main/Screenshots/Spyder_Screenshot%202021-10-16%20163759.png)





  
