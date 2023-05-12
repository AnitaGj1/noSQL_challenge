# noSQL_challenge

### Introduction

In this challenge, I was assigned to evaluate some of the ratings data in order to help journalists and food critics of a food magazine, "Eat Safe, Love" decide where to focus future articles. The data is from the UK Food Standards Agency which evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. 

## Part 1: Database and Jupyter Notebook Set Up

Here I imported the needed libraries: PyMongo and Pretty Print (pprint), imported the data and created the database `uk_food` and collection `establishments`. Assigned the variables and prepared the collection for further use.

## Part 2: Update the Database

Before I can perform any queries or analysis, I had to do some modifications in the database. A new reasturant was added to the database.

![alt text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/added_new_restaurant.png)

The magazine wasn't interested in any establishments within the Dover Local Authority, so I had those removed.

![alt text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/del_Dover.png)

Also, I had to convert some of the number values which were stored as strings, when they should be stored as numbers.

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/converting_datatypes.png)

## Part 3: Exploratory Analysis

In this part, Eat Safe, Love has specific questions they want to be answered, which will help them find the locations they wish to visit and avoid.
Questions to be answered:

>1. Which establishments have a hygiene score equal to 20?

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/hygiene20.png)

>2. Which establishments in London have a RatingValue greater than or equal to 4?

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/London_rating4.png)

>3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/search_from_the_new_restaurant.png)

>4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/localAuthority.png)

![alt_text](https://github.com/AnitaGj1/noSQL_challenge/blob/main/Images/localAuthority_df.png)


NOTE: Worked with the TA for the code to check that the coordinates and rating value are numbers.
