Create a RESTful web service that stores phone book entries in a database called PhoneBookDB and a web client application that consumes this service.  
The web service should output XML.  
Create the PhoneBook database and a data source name for accessing it (as shown in Module 27). 
The database contains one table—PhoneBook—with three columns—LastName, FirstName and PhoneNumber.  
The LastName and FirstName columns store up to 30 characters. The PhoneNumber column supports phone numbers of the form (800) 555-1212 that contain 14 characters.  
Use the PhoneBookDB.sql script provided in the examples folder to create the PhoneBook table. 
Give the client user the capability to enter a new contact (web method addEntry) and to find contacts by last name (web method getEntries).  
Pass only Strings as arguments to the web service. The getEntries web method should return an array of Strings that contains the matching phone book entries.  
Each String in the array should consist of the last name, first name and phone number for one phone book entry. These values should be separated by commas. 

The SELECT query that will find a PhoneBook entry by last name should be: 
 
SELECT LastName, FirstName, PhoneNumberFROM PhoneBook 
WHERE (LastName = LastName) 
 
The INSERT statement that inserts a new entry into the PhoneBook database should be: 
INSERT INTO PhoneBook (LastName, FirstName, PhoneNumber)VALUES (LastName, FirstName, PhoneNumber) 
