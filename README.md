## Product Purchase SQL Assessment
Working with my SQL knowledge and a dataset involving product purchase information, I will answer a series of questions about the data. I'll be using the purchases table from the productpurchases database for all questions.

The fields I'll be working with include the following:

created_at (date)
name (string)
address (string)
state (string)
zipcode (integer)
user_id (integer)

## #1
"Write a query that returns the count for all records in the purchases table."

<img width="500" alt="1" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/0426e5f8-a376-4e84-8e1c-d0fa4d6586c5">

## #2
"Write a query that returns the count of records for the months after May. Store this in an alias named num_after_may."

There's a function EXTRACT() that returns time and date information. Try inserting this line in your query: WHERE EXTRACT (month FROM created_at) > 5.

<img width="497" alt="2" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/5a4e52cb-fde4-4ff8-967f-97b100bea833">

## #3
"Write a query that returns the name of the customer and the state for all the purchases made in Florida."

state = 'FL'

<img width="499" alt="3" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/4277ce4a-9fcd-4fba-8d3f-ecc7afb64a94">

## #4
"Write a query that returns the count of purchases in zipcode 11065."

<img width="500" alt="4" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/55ca05ab-cc4a-45c9-a919-4ad7126144d6">

## #5
"Write a query that returns the count of purchases where the user ID is between 1 and 10 inclusive, and where the states are not Florida or Georgia."

<img width="498" alt="5" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/0204b9fc-5b96-431c-8c0a-15a5b2074162">

## #6
"Write a query that returns the count of purchases from the zip codes 99652, 11065, and 66513."

<img width="500" alt="6" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/7b8474c0-c0df-46a3-bb84-d0035d5e08b2">

## #7
"Write a query that returns the count of all user_id records between 10 and 50, exclusive of the user IDs 20 and 30."

<img width="503" alt="7" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/ce07d246-bb09-45a6-9fd2-bb8068a43cf9">

## #8
"Write a query that returns the name, address, state, and zip code from all purchases.

For the names, return only the first five characters, and display them in all uppercase letters, sorted in alphabetical order."

There are two functions that will help: The UPPER() function converts letters to uppercase. And the function LEFT(field, number of characters) will return the specified number of characters from the left. Try these functions in your SELECT statement.

<img width="501" alt="8" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/5d9b0089-36ea-425b-9d4e-63330535fb72">

## #9
"Write a query that returns a new field called name_date that combines the name and date fields with the labels 'name:' and 'date:'." 
Your first row should look like this:
name: Harrison Jonson; date: 2011-03-16

Hint: Use the CONCAT() function that you learned about to combine the labels with the field names.

<img width="501" alt="9" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/3b4d47b8-3382-4ee9-84fb-53995d024fdf">

## #10
"Find if any of the zip codes are missing (null). Write a query that finds all of the null zip codes and list this by name."

<img width="498" alt="10" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/de0116f7-4807-4f7a-a285-6b4ea9df88f3">

## #11
"Write a query that returns user_id, created_at, name, and address for all records where the state is Georgia and user_id is 18, or where the user_id is 20 with any state. Order the list by the date that the order was created from newest to oldest."

<img width="499" alt="11" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/227de2f6-b1d8-464b-91d0-05c660da17c2">

## #12
"Write a query that returns name, address, state, and zipcode where (1) the state is Illinois, (2) or the zip code is between 30000 and 80000, and the first two characters in the address are 23 or 12, and the state is either Colorado, Texas, or Wyoming."

<img width="501" alt="12" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/d1f3f54a-5e24-492c-8438-2a0e47b492ac">

## #13
"Write a query that returns all the records for the top 10 purchases with the highest zip code number (descending order)."

<img width="499" alt="13" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/cad6d528-3b7e-4f0a-9a3c-e19880250441">

## #14
"Write a query that returns all the records of purchases where the buyer's first name starts with a capital S. Sort the list by name."

<img width="504" alt="14" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/90c542ab-a56f-4b98-b3f4-6cd9f8689500">

## #15
"Write a query that returns all the records of purchases where the buyer's first name starts with a capital S or a capital T. Sort the list by name."

<img width="503" alt="15" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/5597aab3-c53d-49ae-8e55-4859224f3e2c">

## #16
"Write a query that returns the count of records where the size of the name field is greater than or equal to 15 characters."

There's a function LENGTH() that returns the size of a field, like this: LENGTH(field). Try this function with your WHEREclause.

<img width="498" alt="16" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/2d3667a7-8d13-48f0-95da-60b937e654f3">

## #17
"Write a query that returns the count of all records where state starts with a letter greater than M, zipcode is greater than 50000, and user_id is greater than 10 (all non-inclusive)."

<img width="501" alt="17" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/20c5e123-688b-4bed-a85c-44a2d0f8563f">

## #18
"Write a query that returns all records where the buyer's name has a lowercase e in its third position."

<img width="502" alt="18" src="https://github.com/romaoeh/Product-Purchase-SQL/assets/131217181/42cb6804-affa-49c3-887c-f33f0356a70d">

