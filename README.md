# Animal-Shelters-SQL-Certification
SQL project from Data Camp exams
this porject using SQL to explore shelter data 
# project Overview
As a data analyst in the animal welfare department. In preparation for next year's budget, the head of department would like to know the total cost to shelter animals, broken down by each animal type and size combination .
# requirements
prepare a table that contains this information.
- The total cost to shelter an animal for the year is calculated as the sum of three factors: the size and animal type, the age, and the location.
The base cost of sheltering an animal is based upon its size and type. The costs per animal type and size are contained in the size_costs table. The criteria for classifying size has recently been updated, and so you will need to categorize animals based upon the following table:

| | Small | Medium | Large |
| :---: | :---: | :---: | :---: |
| Dog |<= 10 lbs|10 lbs < and <= 30 lbs|30 lbs <|
| Cat |<= 5 lbs| 5 lbs < and <= 7 lbs|7 lbs <|
| Bird|<= 0.7 lbs|0.7 lbs < and <= 1.1 lbs|1.1 lbs <|
- Older animals cost more, and so an age cost (contained in the age_costs table) is added. Each animal's age should be calculated as the age by the end of the year (December 31st, 2021).
- There is a location cost depending on where the animal is sheltered (contained in the location_costs table).
- The calculation should not include animals that have been sponsored by private charities (sponsored animals are listed in the sponsored_animals table).

For future visualization purposes, you will also need to include a percentage column in your result. This percentage should reflect the fraction of the total cost to be allocated to each animal and size combination.

Order query by animal type in alphabetical order, and then size (in order from small to large). Percentage should be expressed as a number rounded to two decimal places (e.g. 50.25% becomes 50.25). 
# output
query will need to return a table that resembles the following, including the same column names:

| animaltype |	size|	total |	percentage |
| :---: | :---: | :---: | :---: |
| bird	| small	| ???	| ??? |
| bird	| medium | ???	| ??? |
| bird	| large	| ??? |	??? |
| cat | ??? | ??? | ??? |
| ???	| ??? |	???	| ??? |

# Running the program in your computer 
- create the database on your server using pgadmin or any other program , code in createdb.sql file
- load the tables from the file using the sql code on createdb.sql file.
- create the magic tool %sql and connect to the server
- run the code in the notebook

# result
|animaltype|	size	|total	|percentage|
| :---: | :---: | :---: | :---: |
|Bird	|Small	|1615	|0.05|
|Bird	|Medium	|3460	|0.10|
|Bird	|Large	|7770	|0.22|
|Cat	|Small	|518015	|14.90|
|Cat	|Medium	|250575	|7.21|
|Cat	|Large	|439490	|12.64|
|Dog	|Small	|336530	|9.68|
|Dog	|Medium	|941895	|27.09|
|Dog	|Large	|977665	|28.12|
