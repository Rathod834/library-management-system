# library-management-system

    This is a library management API Backend for the management of user and the books

# Roots and the Endpoints

## /user
    GET: Get all the list of user in the system
    POST: Create/Register a new user

## /user/{id}
    GET: Get a user by their ID
    PUT: Updating a user by their ID
    DELETE: Delating a user by their ID (Check if the user still has an issued book) && {is there any fine/penalty to be collected}

## /user/subcription-details/{id}
    GET: Get a user subcription details by their ID
        >> Date of Subcription
        >> Valid till?
        >> Fine if any?

## /books
    GET: Get all the books in the system
    POST: Add a new book to the system

## /book/{id}
    GET: Get a book by its ID
    PUT: Update a book by its ID
    DELETE: Delete a book by its ID

## /book/issued
    GET: Get all the issued books

## /book/issued/withFine
    GET: Get all issued books with their fine amount

### Subcription Types
    >> Basic (3 Month)
    >> Standard (6 Month)
    >> Premium (12 Month)


>> if a user missed the renewal date, then user should be collected with $100
>> if a user missed his subcription, then user is expected to pay $100
>> if a user missed both renwal & subcription, then the collected amount should be $200


## Commands:
    npm init
    npm i express
    npm i nodemon --save-dev

    npm run dev

    To restore node_modules and package-lock.json --> npm i/npm install

    