## Total number of Publishers
`SELECT COUNT( DISTINCT Publisher) as Publishers_total
FROM Books`

![image](https://user-images.githubusercontent.com/108747030/189496758-ae03cdd3-8a64-4034-beb1-0754e2ef64a9.png)

## Total number of Authors
`SELECT COUNT( DISTINCT Book_author) as Authors_total
FROM Books`

![image](https://user-images.githubusercontent.com/108747030/189496735-5f14ef5e-1074-46c5-b350-83e9728a6569.png)

## Book Publication Count by Publisher (showing first 5)
`SELECT COUNT (Book_title) AS Book_Publication_by_Publisher, Publisher
FROM Books
GROUP BY Publisher
ORDER BY Book_Publication_by_Publisher DESC`

![image](https://user-images.githubusercontent.com/108747030/189496715-0b999748-3500-4951-a322-25c6d75f46eb.png)

## Book Publication Count by Year (showing first 5)
`SELECT COUNT (Book_title) AS Total_Book_Publication, Year_of_Publication
FROM Books
GROUP BY Year_of_Publication
ORDER BY Total_Book_Publication DESC`


![image](https://user-images.githubusercontent.com/108747030/189496673-2ca63228-6118-4eee-acef-77600687b9de.png)

## Book Publication  Count by Author (showing first 5)
`SELECT COUNT (Book_author) AS Publications_by_author, Book_author
FROM Books
GROUP BY Book_author
ORDER BY Publications_by_author DESC`

![image](https://user-images.githubusercontent.com/108747030/189496551-265ce874-c4ff-4fc5-84a0-9fb8e076696f.png)

## Number of Books Published Between 2000 and 2005

**Total Books Published**

`SELECT COUNT(Book_title) AS Total_Publication, Year_of_Publication
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005`

![image](https://user-images.githubusercontent.com/108747030/189546568-ade9c4a2-03c8-4b32-ad10-a7ab2f4b6820.png)

**Seggregated by Year**

`SELECT COUNT(Book_title) AS Total_Publication, Year_of_Publication
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005
GROUP BY Year_of_Publication`

![image](https://user-images.githubusercontent.com/108747030/189546605-0c53b3b4-6d0a-484a-8d8b-a528a367aac4.png)


## Publisher that Most published Between 2000 and 2005

`SELECT COUNT(Book_title), Year_of_Publication, Publisher
FROM Books
WHERE Year_of_Publication BETWEEN 2000 and 2005
GROUP BY Publisher
ORDER BY COUNT(Book_title) DESC`

![image](https://user-images.githubusercontent.com/108747030/189547094-e857b0bb-b254-4f37-a28c-c2e4dd80c88d.png)


# UPDATE

# TRUNCATE

# DELETE




SQLLiteStudio (3.3.3)
