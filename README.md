# Sakila-DVD-Rental-database-Project
Analysis of the Sakila DVD Rental database using SQL

## Introduction

In this project, we have queried the Sakila DVD Rental database. The Sakila Database holds information about a company that rents movie DVDs. For this project, we have queried the database to gain an understanding of the customer base, such as what the patterns in movie watching are across different customer groups, how they compare on payment earnings, and how the stores compare in their performance. For assistance in the queries, the schema for the DVD Rental database is provided below

(http://www.postgresqltutorial.com/postgresql-sample-database/)

## Local Environment Setup
Follow the steps provided below to setup the local environment with **PostgreSQL** and database

**Step 1. Downloading PostgreSQL**
First, we will need to install PostgreSQL on your local machine. The instructions below provide detailed description of the steps we need to take.

**Installing PostgreSQL for Windows:**
http://www.postgresqltutorial.com/install-postgresql/

**Installing PostgreSQL for Mac OS:**
https://www.postgresql.org/download/macosx/

**Note:** We need to write down the database superuser (postgres) password as we will need it to create the Sakila database once we have installed the PostgreSQL server.

**Step 2. Downloading Sakila database**
Once PostgreSQL server is installed, we will need to download the Movie database from this page: [PostgreSQL Sample Database](http://www.postgresqltutorial.com/postgresql-sample-database/)

Scroll down and click on the orange "Download DVD Rental Sample Database" button.

This will download a zipped file, and you will need to extract the `dvdrental.tar file`.

Step 3. Loading database
The next step is to load the DVD Rental database into our PostgreSQL server on our machine. We recommend using the **PgAdmin tool**. We can find the instructions to do so on the following link: [Load PostgreSQL Sample Database](http://www.postgresqltutorial.com/load-postgresql-sample-database/).

The instructions are down ⅓ on this page under the header **“Load the DVD Rental database using pgAdmin tool”** .

Now, we need to follow the instructions all the way through the header titled **"Verify the loaded sample database."**

Once we have followed the instructions through the end of **"Verify the loaded sample database."**, we have now loaded the `dvdrental` sample database into our local PostgreSQL database server.

**Step 4. Connecting back to the PostgreSQL server:**
Now, we will relaunch PgAdmin III and click on the PostgreSQL server within the Object browser and enter our superuser (postgres) password.

**Step 5. Connecting to the DVD rental database:**
Next, we will click on the plus sign next to Databases to access the DVD rental database.

**Step 6. Choose the DVD Rental database**
Choose the `dvdrental` database under Databases.

We are now linked to the DVD rental database.

**Step 7. Running Queries on your dvdrental database**
Now, we are ready to run some queries. For that, we need to click on the SQL icon with a magnifying glass

## Questions to work upon for analysis

**Question 1**
We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.

**Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.**

**Question 2**
We want to find out how the two stores compare in their count of rental orders during every month for all the years we have data for. 

 **Write a query that returns the store ID for the store, the year and month and the number of rental orders each store has fulfilled for that month. Your table should include a column for each of the following: year, month, store ID and count of rental orders fulfilled during that month.** 

**Question 3**
We would like to know who were our top 10 paying customers, how many payments they made on a monthly basis during 2007, and what was the amount of the monthly payments.
 **Can you write a query to capture the customer name, month and year of payment, and total payment amount for each month by these top 10 paying customers?**

**Question 4**
Finally, for each of these top 10 paying customers, I would like to find out the difference across their monthly payments during 2007. **write a query to compare the payment amounts in each successive month.** Repeat this for each of these 10 paying customers. Also, it will be tremendously helpful if you can identify the customer name who paid the most difference in terms of payments.
