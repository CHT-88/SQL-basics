## Total number of Publishers
`SELECT COUNT( DISTINCT Publisher) as Publishers_total
FROM Books`

![image](https://user-images.githubusercontent.com/108747030/189496758-ae03cdd3-8a64-4034-beb1-0754e2ef64a9.png)

## Total number of Authors
`SELECT COUNT( DISTINCT Book_author) as Authors_total
FROM Books`

![image](https://user-images.githubusercontent.com/108747030/189496735-5f14ef5e-1074-46c5-b350-83e9728a6569.png)

## Book Publication Count by Publisher (showing first 5)
`SELECT COUNT (Book_title) AS Books_Published, Publisher 
FROM Books 
GROUP BY Publisher ORDER BY Books_Published DESC`

![image](https://user-images.githubusercontent.com/108747030/189618598-dc52a6f1-49a2-4cdd-bfbd-12a2e51ece56.png)

## Book Publication Count by Year (showing first 5)
`SELECT COUNT (Book_title) AS Books_Published, Year_of_Publication
FROM Books
GROUP BY Year_of_Publication
ORDER BY Books_Published DESC`

![image](https://user-images.githubusercontent.com/108747030/189618475-5acc9177-ff86-4ac5-934f-229de514ce3d.png)

## Book Publication  Count by Author (showing first 5)
`SELECT COUNT (Book_author) AS Books_Published, Book_Author
FROM Books
GROUP BY Book_author
ORDER BY Books_Published DESC`

![image](https://user-images.githubusercontent.com/108747030/189619129-7cfee716-1d6e-40f9-8ac7-256fdc20271a.png)

## Number of Books Published Between 2000 and 2005

**Total Books Published**

`SELECT COUNT(Book_title) AS Total_Publication
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005`

![image](https://user-images.githubusercontent.com/108747030/189616496-59fa6376-be61-4b61-9174-8a68d2b1dea4.png)

**Seggregated by Year**

`SELECT COUNT(Book_title) AS Total_Publication, Year_of_Publication
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005
GROUP BY Year_of_Publication`

![image](https://user-images.githubusercontent.com/108747030/189546605-0c53b3b4-6d0a-484a-8d8b-a528a367aac4.png)


## Publisher that Most published Between 2000 and 2005

`SELECT COUNT(Book_title) AS Books_Published, Publisher 
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005
GROUP BY Publisher 
ORDER BY Books_Published DESC`

![image](https://user-images.githubusercontent.com/108747030/189620804-89c13656-3b2f-413e-ba84-2f0420e8e42d.png)


# UPDATE
`UPDATE Books
SET Book_Author = 'Mark Morford'
WHERE ISBN = 195153448`

Updated value:
![image](https://user-images.githubusercontent.com/108747030/189623051-06ae3174-d8b6-48cb-9b31-3eae8d160457.png)

# TRUNCATE TABLE
Removing data rows from the table.

`TRUNCATE TABLE Books`

# DELETE TABLE
Removing data rows from the table Published before 1990.

`DELETE FROM Books
WHERE Year_of_Publication < 1990`

# DROP TABLE
Removing all the data in the table and the table itself.
`DROP TABLE Books`



SQLLiteStudio (3.3.3)
