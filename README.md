# ChicagoCrimeData

In this project, we will explore Chicago Crime Dataset and implement a relational database for storing the data

1. Identify the features (attributes) in Chicago Crime dataset and design an entity-relationship model
2. Refine the model and convert each relation to BCNF
3. Using DDL implement the relations in a Postgres server
4. Load the given data to the relations
5. Execute some interesting queries on the relations


DATA EXPLORATION:


# What did you learn from the data set?
This dataset contains multiple values and there are multiple dependencies present in this dataset. The location can be known if we know the values of longitude and latitude and vice versa. The same thing goes with the date attribute and the year attribute. The table can be easily decomposed into a smaller and simple table which presents the data clearly rather than displaying large amount of data.

# Data types of the attributes? How to deal with the date information? 
The dataset contains a mixture of categorical and numerical data. There are only few columns which contains multiple values which needs to be changed through the process of normalization. The date attribute contains the date and time, a new time column can be created and the time can be seperated from the date column. Even the location attribute contains both longitude and latitude together.

# Any missing values?
There are missing values present in the location attribute including the X-coordinate and the Y coordinate.

# Do you see redundancy? Many repetive values in some columns. How to deal with that? Creating a new table?
Yes data redudancy exists in this table, most of the rows contains same data value and the redudancy could be reduced by assiging seperate ID for each value and creating a new table where each and every data cell is assigned with the id which corresponds to the data in the new table

# Any outside information to link back to this data?
Each IUCR is supposed to correspond to a distinct FBI Code. However, in our data, this appears to be violated in one case, with IUCR code 2093, which takes on two different FBI Codes



Developed five distinct and useful queries that could be potentially used for policing planning, policy making, citizen awareness, etc.
Each query has documentation to explain what this query is looking for and why it is meaningful for what purposes.
