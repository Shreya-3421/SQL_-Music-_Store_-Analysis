# SQL_-Music-_Store_-Analysis

# Overview
The **SQL Music Store** project is a relational database designed to manage a music store's inventory, sales, and customer transactions efficiently. It includes structured tables to store information about albums, artists, tracks, customers, employees, invoices, and playlists.

# Features
- **Albums Management**: Stores details of albums, including titles and associated artists.
- **Artists Database**: Maintains records of music artists.
- **Tracks Information**: Contains details about individual tracks, including duration, genre, and media type.
- **Customer Management**: Tracks customer details and their purchases.
- **Employee Records**: Maintains employee information and reporting structure.
- **Invoice System**: Manages sales transactions, linking customers with their purchases.
- **Playlists**: Stores curated playlists and their associated tracks.

# Database Schema
The database consists of the following tables:
- Artist (ArtistId, Name)
- Album (AlbumId, Title, ArtistId)
- Track (TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, UnitPrice)
- MediaType (MediaTypeId, Name)
- Genre (GenreId, Name)
- Playlist (PlaylistId, Name)
- PlaylistTrack (PlaylistId, TrackId)
- Employee (EmployeeId, LastName, FirstName, Title, ReportsTo, BirthDate, HireDate, Address, City, State, Country, PostalCode, Phone, Fax, Email)
- Customer (CustomerId, FirstName, LastName, Company, Address, City, State, Country, PostalCode, Phone, Fax, Email, SupportRepId)
- Invoice (InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total)
- InvoiceLine (InvoiceLineId, InvoiceId, TrackId, UnitPrice, Quantity)

# SQL Queries Included
## **Question Set 1 **
1. Who is the senior-most employee based on job title?
2. Which countries have the most invoices?
3. What are the top 3 values of total invoice amounts?
4. Which city has the best customers? We would like to throw a promotional music festival in the city where we made the most money. Write a query that returns one city that has the highest sum of invoice totals. Return both the city name & sum of all invoice totals.
5. Who is the best customer? The customer who has spent the most money will be declared the best customer. Write a query that returns the person who has spent the most money.

## **Question Set 2 **
1. Write a query to return the email, first name, last name, & genre of all rock music listeners. Return your list ordered alphabetically by email starting with 'A'.
2. Let's invite the artists who have written the most rock music in our dataset. Write a query that returns the artist name and total track count of the top 10 rock bands.
3. Return all the track names that have a song length longer than the average song length. Return the name and milliseconds for each track. Order by the song length with the longest songs listed first.

## **Question Set 3 **
1. Find how much amount each customer spent on artists. Write a query to return customer name, artist name, and total spent.
2. We want to find out the most popular music genre for each country. We determine the most popular genre as the genre with the highest amount of purchases. Write a query that returns each country along with the top genre. For countries where the maximum number of purchases is shared, return all genres.
3. Write a query that determines the customer who has spent the most on music for each country. Write a query that returns the country along with the top customer and how much they spent. For countries where the top amount spent is shared, provide all customers who spent this amount.

# Technologies Used
- SQL (Structured Query Language)
- MySQL/PostgreSQL (Database Management System)


