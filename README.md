# JSON Web Server Boilerplate

## Available scripts

` npm start `
Starts the json server

## Consuming

REST API for methods: GET, POST, PUST, PATCH, DELETE

Urls are: `http://localhost/<Json_Collection_Name>`

Example:
#### File json.db
> {
>   "users":[{
>     "id":1,
>     "name":"facundo",
>     "password":"facundo123"
>   }]
> }

GET to `http://localhost/users`
Result:
> [
>   {
>     "id": 1,
>     "name": "facundo",
>     "password": "facundo123"
>   }
> ]
> 
# JSON Web Server Auth Boilerplate

Any of the following routes registers a new user :

POST /register
POST /signup
POST /users
email and password are required in the request body :

POST /register
{
    "email":"fcristaldo@altimetrik.com",
    "password":"facu123"
}

Response:
{
"accessToken": "...."
}

POST /login
{
    "email":"fcristaldo@altimetrik.com",
    "password":"facu123"
}

Response:
{
"accessToken": "...."
}

