# DISTINCT

## Total number of Publishers
`SELECT COUNT( DISTINCT Publisher) as Publishers_total
FROM Books`

Result: Publishers_total = 364

## Total number of Authors
`SELECT COUNT( DISTINCT Book_author) as Authors_total
FROM Books`

Result:
Total of different authors = 777

# COUNT
`SELECT COUNT (Book_title) AS Book_Publication_by_Publisher, Publisher
FROM Books
GROUP BY Publisher
ORDER BY Book_Publication_by_Publisher DESC`

Result: 
Top 5 Total of Book Publication by Publisher
Book_Publication_by_Publisher	Publisher
49	Ballantine Books
26	Pocket
26	Perennial
24	Signet Book
24	Berkley Publishing Group


`SELECT COUNT (Book_title) AS Total_Book_Publication, Year_of_Publication
FROM Books
GROUP BY Year_of_Publication
ORDER BY Total_Book_Publication DESC`

/Result:
Showing the Top 5 Number of Publication by Year
Total_Book_Publication	Year_of_Publication
106	2002
93	2000
79	2001
77	1999
69	2003



`SELECT COUNT (Book_author) AS Publications_by_author, Book_author
FROM Books
GROUP BY Book_author
ORDER BY Publications_by_author DESC`

Result: Showing Top 5 Authors with most Publications
Publications_by_author	Book_author
10	Jonathan Pearce
8	John Grisham
8	James Patterson
7	Terry Pratchett
7	Stephen King


SQLLiteStudio (3.3.3)
