## Laravel Sanctum 

What is Laravel Sanctum ?
Laravel Sanctum provides a featherweight authentication system for SPAs (single page applications), mobile applications, and simple, token based APIs. Sanctum allows each user of your application to generate multiple API tokens for their account. These tokens may be granted abilities / scopes which specify which actions the tokens are allowed to perform..


### API Login

````
curl --location --request POST 'http://127.0.0.1:8000/api/login' \
--header 'Content-Type: application/json' \
--data-raw '{
    "email": "joaquin@rivera.com",
    "password": "1234"
}'
````

### API List Users

````
curl --location --request GET 'http://127.0.0.1:8000/api/users' \
--header 'Authorization: Bearer valor_token'
````
