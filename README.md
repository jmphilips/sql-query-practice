# sql-query-practice

1)  SELECT Customer.FirstName || ' ' || Customer.LastName As Name,
            Customer.CustomerId, 
            Customer.Country
    FROM    Customer
    WHERE Customer.Country IS NOT 'USA'

2) SELECT Customer.FirstName || ' ' || Customer.LastName As Name,
                    Customer.CustomerId, 
                    Customer.Country
            FROM    Customer
            WHERE Customer.Country IS 'Brazil

3) SELECT Customer.FirstName || ' ' || Customer.LastName As 'Name'
            Invoice.InvoiceId,
            Invoice.InvoiceDate,
            Invoice.BillingCountry,
    FROM Invoice 
    JOIN Customer ON Invoice.CustomerId = Customer.Customer.Id
    WHERE Customer.Country = 'Brazil'

4) SELECT FirstName || " " || LastName As "Name"
	FROM Employee
	WHERE Title = "Sales Support Agent"

5) SELECT DISTINCT "BillingCity" FROM Invoice

6) SELECT * FROM Invoice 
	WHERE "BillingCountry" = "Brazil"