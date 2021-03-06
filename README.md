# Hair Salon app

#### An Epicodus exercise in Database Design, 06.09.17

#### **By Nick Wise***

## Description

This web application will allow a Owner to enter, edit and delete an employed Stylist. The Stylist can look up the names of the Clients they have and add, edit, or remove the specified Client. This application is meant for Stylist mainly to keep track of their Clients and view other Stylist Clients.

| Hair Salon behavior | input  | output  |
|---|---|---|
| Program will allow Employee to see list of stylist | nancy, josh, jenny | nancy, josh, jenny | - Need a page that displays all currently employed stylists.
| Employee can look under a specific stylist to see there details and clients |jenny | Name: "jenny" Clients: "Frank", "Bob", "Sally" | - on click route to id of selected stylist
| Owner can add a new stylist | "Sally" | "Sally" | - form that gets the id and name of the new stylist and routing within our save and find methods so they can be stored in databaseS
| Stylist can add new clients to there list of clients | add Client: "James" to Stylist: "Jenny" | Jennys Clients : "James", "Bob", "Jessica"| - one to many relation ship where the client has a stylist Id attached to their name so we can add multiple clients to a single stylist.
| Stylist can update client to there list of clients name| update Client: "James" to Client: "Jenny" | Update "James" to "Jenny"| - Update and Patch methods allow us to update user information.
| Stylist can delete  clients to there list of clients | delete Client: "James" to Stylist: "Jenny" | Jennys Clients : "Bob", "Jessica"| - one to many relation ship where the client has a stylist Id attached to their name so we can delete a client.


## Setup/Installation Requirements

https://github.com/YcleptInsan/Salon
1. Click the "clone" button and copy the link.
2. In your computers terminal type "git clone" & paste the copied link.
3. Once downloaded you can open the index.html file in the browser of your choice.
4. You can view the code using the text editor of your choice as well.
5. In PowerShell type: sqlcmd -S "(localdb)\mssqllocaldb",
6. Next, type SQLCMD: > CREATE DATABASE salon; > GO > USE salon; > GO > CREATE TABLE client (id INT IDENTITY(1,1), name VARCHAR(255), stylist_id INT); > CREATE TABLE stylist (id INT IDENTITY(1,1), name VARCHAR(255)); > GO. 
7. To view the page, you need to initialize the local server by typing dnx kestrel in your powershell window. Next, you will need to input http://localhost:5004/ into your prefered browser to view the actual page content.   

## Known Bugs

* No known bugs


## Support and contact details

If you have any issues or have questions, ideas, concerns, or contributions please contact any of the contributors through Github.

## Technologies Used

* HTML
* JSON
* C#
* Nancy
* Razor
* xUnit
* SQL Server management 2016
* ADO.NET

### License
This software is licensed under the MIT license.

Copyright (c) 2017 **Nick Wise**
