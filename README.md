# Animal-Shelters-SQL-Certification
SQL project from Data Camp exams
this porject using SQL to explore shelter data 
# project Overview
As a data analyst in the animal welfare department. In preparation for next year's budget, the head of department would like to know the total cost to shelter animals, broken down by each animal type and size combination . task is to prepare a table that contains this information.

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

