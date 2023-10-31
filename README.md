# hasian-betest

## Project Structure
This repository is organized into three main folders:

db-hasian-betest
this folder contains sample of db using mongodb

ms-hasian-betest
this folder contains rest api that connected to mongodb

redis-hasian-betest
this folder contains of redis that would perform cached data from ms-hasian-betest


## Installation
1. clone this repo: git clone https://github.com/yourusername/hasian-betest.git
2. import the database from db-hasian-betest
3. go to directory ms-hasian-betest and perform npm i && npm start
4. go to directory redis-hasian-betest and perform npm i && npm start

## Usage
POST http://172.104.50.86:3000/auth - to generate token
POST http://172.104.50.86:3000/users 
Body:
userName - string 
accountNumber - string, unique
emailAddress - string
identityNumber - string, unique
GET http://172.104.50.86:3000/users/identity-number - to find by identity-number
GET http://172.104.50.86:3000//users/account-number - to find by account-number
GET http://172.104.50.86:3000//users/id - to find by id
PUT http://172.104.50.86:3000//users/id
userName - string 
accountNumber - string, unique
emailAddress - string
identityNumber - string, unique
DELETE http://172.104.50.86:3000/users/id -  to delete user by id


