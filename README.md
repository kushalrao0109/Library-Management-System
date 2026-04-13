# Library-Management-System

    This is the Library Management API backend for the management of user and the books 

# Routes and the Endpoints

## /users 
GET: Get all the list of the users in the system 
POST: Create/Register a new user 

## /users/{id}
GET: Get a user by their ID 
PUT: Updating a user by their ID 
DELETE: Deleting a user by their ID (Check if the user still has an issued an book) && {is there any fine/penalty to be collected}

## /users/subcription-details/{id}
GET: Get a user sudcription details by their ID 
    >> Date of Subcription 
    >> Vaild till?
    >> Fine if any?

## /books
GET: Get all the books in the system 
POST: Add a new book to the system 

## /books/{id}
GET: Get a book by its ID 
PUT: Update a book by its ID 
DELETE : Delete a book by its ID 

## /books/issued
GET: Get all the issued books 

## /books/issued/withFine
GET: Get all the issued books with their Fine Amount 

## Subcription Types 
    >> Basic (3 months)
    >> Standard (6 months)
    >> Premium (12 months) 

>> If a user misses the renewal date, then user should be collected with $100
>> If a user misses the Subcription, then the user is expected to pay $100
>> If a user misses both renewal and Subcription, then the collected amount should be $200 

## Commands 
npm init 

npm i express 

npm i nodemon --save-dev 

npm run dev 

To restore node_module and package-lock.json --> npm i/npm install 
