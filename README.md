# sql-query-practice

1. Provide a query showing Customers (just their full names, customer ID and country) who are not in the US.
```
SELECT Customer.FirstName || ' ' || Customer.LastName As Name,
            Customer.CustomerId, 
            Customer.Country
FROM    Customer
WHERE Customer.Country IS NOT 'USA'
```
2. Provide a query only showing the Customers from Brazil.
```
SELECT Customer.FirstName || ' ' || Customer.LastName As Name,
                    Customer.CustomerId, 
                    Customer.Country
        FROM    Customer
        WHERE Customer.Country IS 'Brazil
```
3. Provide a query showing the Invoices of customers who are from Brazil. The resultant table should show the customer's full name, Invoice ID, Date of the invoice and billing country.
```
SELECT Customer.FirstName || ' ' || Customer.LastName As 'Name'
            Invoice.InvoiceId,
            Invoice.InvoiceDate,
            Invoice.BillingCountry,
        FROM Invoice 
        JOIN Customer ON Invoice.CustomerId = Customer.Customer.Id
        WHERE Customer.Country = 'Brazil'
```
4. Provide a query showing only the Employees who are Sales Agents.

```
SELECT FirstName || " " || LastName As "Name"
	FROM Employee
	WHERE Title = "Sales Support Agent"
```


5. Provide a query showing a unique list of billing countries from the Invoice table.\

```
SELECT DISTINCT "BillingCity" FROM Invoice
```


6. Provide a query showing the invoices of customers who are from Brazil.

```
SELECT * FROM Invoice 
        WHERE "BillingCountry" = "Brazil"
```


7. Provide a query that shows the Invoice Total, Customer name, Country and Sale Agent name for all invoices and customers.

8. Provide a query that shows the Invoice Total, Customer name, Country and Sale Agent name for all invoices and customers.
9. How many Invoices were there in 2009 and 2011? What are the respective total sales for each of those years?
10. Looking at the InvoiceLine table, provide a query that COUNTs the number of line items for Invoice ID 37.
11. Looking at the InvoiceLine table, provide a query that COUNTs the number of line items for each Invoice. HINT: GROUP BY
12. Provide a query that includes the track name with each invoice line item.
13. Provide a query that includes the purchased track name AND artist name with each invoice line item.
14. Provide a query that shows the # of invoices per country. HINT: GROUP BY
15. Provide a query that shows the total number of tracks in each playlist. The Playlist name should be include on the resultant table.
16. Provide a query that shows all the Tracks, but displays no IDs. The resultant table should include the Album name, Media type and Genre.
17. Provide a query that shows all Invoices but includes the # of invoice line items.
18. Provide a query that shows total sales made by each sales agent.
19. Which sales agent made the most in sales in 2009?
20. Which sales agent made the most in sales in 2010?
21.Which sales agent made the most in sales over all?
22.Provide a query that shows the # of customers assigned to each sales agent.
23.Provide a query that shows the total sales per country. Which country's customers spent the most?
24.Provide a query that shows the most purchased track of 2013.
25.Provide a query that shows the top 5 most purchased tracks over all.
26.Provide a query that shows the top 3 best selling artists.
27.Provide a query that shows the most purchased Media Type.