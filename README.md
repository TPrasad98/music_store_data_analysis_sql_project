
# Music Store Data Analytics Project

This project focuses on analyzing data from a music store database to derive insights and answer various business questions. It includes SQL queries for data analysis and is divided into three question sets based on difficulty: Easy, Moderate, and Advanced.

## Table of Contents

- [Question Sets](#question-sets)
- [Approach to Solve](#approach-to-solve)
- [Contributing](#contributing)
- [License](#license)

## Question Sets

### Easy Questions

1. **Senior Most Employee (Based on Job Title):**
   - Use the `employee` table.
   - Retrieve the job titles and sort them by hierarchy level (assuming `levels` represents job hierarchy).
   - Select the top record after sorting.

2. **Countries with the Most Invoices:**
   - Use the `invoice` table.
   - Count the number of invoices for each country using `GROUP BY`.
   - Order the result by the count in descending order.

3. **Top 3 Values of Total Invoice:**
   - Use the `invoice` table.
   - Select the `total` column and order it in descending order.
   - Limit the result to the top 3 rows.

4. **City with the Best Customers:**
   - Use the `invoice` table and possibly join with other tables to get city information.
   - Group the data by city.
   - Sum the total invoice amounts for each city.
   - Select the city with the highest sum of invoice totals.

5. **Best Customer (Based on Spending):**
   - Use the `customer` and `invoice` tables.
   - Join the tables on the `customer_id` column.
   - Group the data by customer.
   - Sum the total spending for each customer.
   - Select the customer with the highest total spending.

### Moderate Questions

1. **Rock Music Listeners:**
   - Join `customer`, `invoice`, `invoiceline`, and `track` tables.
   - Filter tracks with the genre 'Rock'.
   - Retrieve unique email, first name, and last name of customers.

2. **Top Rock Bands (Based on Track Count):**
   - Join `track`, `album`, and `artist` tables.
   - Filter tracks with the genre 'Rock'.
   - Count the number of tracks for each artist.
   - Order the result by the track count and limit to top 10.

3. **Tracks with Length Longer Than Average:**
   - Use the `track` table.
   - Calculate the average length of all tracks.
   - Select tracks with lengths greater than the average.
   - Order the result by track length in descending order.

### Advanced Questions

1. **Amount Spent by Each Customer on Artists:**
   - Use `invoice`, `invoiceline`, `track`, `album`, `artist`, and `customer` tables.
   - Determine the artist with the highest total sales.
   - Identify the customers who spent the most on this artist.

2. **Most Popular Music Genre by Country:**
   - Use `invoice_line`, `customer`, `track`, and `genre` tables.
   - Count the purchases for each genre in each country.
   - Determine the most popular genre for each country.

3. **Customer Spending on Music by Country:**
   - Use `invoice`, `customer`, and other related tables.
   - Group the data by country and customer.
   - Calculate the total spending for each customer in each country.
   - Identify the top spending customer(s) for each country.

## Approach to Solve

Each question set involves understanding the data schema, joining relevant tables, aggregating data as needed, and applying appropriate sorting and filtering criteria to derive meaningful insights from the dataset.

For detailed approaches to solve each question, please refer to the [Approach to Solve](#approach-to-solve) section in the README file.

## Contributing

Contributions are welcome! Feel free to submit pull requests or open issues for any improvements or new features.

## Database and Tools
* Postgre SQL
* PgAdmin4

Schema- Music Store Database  
![MusicDatabaseSchema](https://github.com/TPrasad98/music_store_data_analysis_sql_project/blob/main/MusicDatabaseSchema.png)

## Special Thanks

A special thanks to [Rishab Sharma](https://github.com/rishabhnmishra) for his invaluable guidance and support .


