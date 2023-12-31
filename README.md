# Heineken Sales Dashboards 
This is the final assignment using Power BI, from the Data Visualization course at the Big Data &amp; Analytics Masters @ [EAE](https://www.eae.es/) class of 2021.
The assignment uses mocked-up data as input provided by the professor:
* *.txt files in comma-separated-values format, that mimic Heineken Sales data from years 2015 and 2016
![image](https://user-images.githubusercontent.com/11904085/123307883-4d287200-d523-11eb-9f63-4594f4517122.png)
*  *.txt files in comma-separated-values format, that mimic Heineken Sales Budget data from the same time period.
* *.txt files in comma-separated-values format, that mimic Nielsen overall market Sales data from the same time period.
* *.xls files that represent Customer, Product, and Salesman master data.
The assignment's purpose is to provide sales insights and recommendations, backed up by visualizations.



## Highlights
### Data Cleansing
* Removed exact duplicates creating a row hash identity column.
* Remove rows having alphanumeric Product Codes, as they were proven invalid.
### Dimension Data Customization
The input data was generic, it was only relevant for us to the fact tables measures and master data ids. 
So, on top of those master data records, we customized attributes such as codes, names, and pictures, resulting in an OLAP Snowflake schema, where there are auxiliary tables to the dimensions to store those customizations such as:
* Customer Name
* Product Brand, Capacity, and Container Type 
* Account Manager Name
* Director Name & Pictures

![image](https://user-images.githubusercontent.com/11904085/123308110-9082e080-d523-11eb-85d8-9b120008ccac.png)

### Sales vs Budget Dashboard
![image](https://user-images.githubusercontent.com/11904085/123312254-5ec04880-d528-11eb-8fd6-2f8399c6e8cc.png)


