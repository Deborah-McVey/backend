# README

https://www.youtube.com/watch?v=YA0WGSTZ1P4

"How to build ruby on rails rest api crud | rails 7 restful api | rails api crud" video by TechWebDocs on YouTube

began document with the command: rails new backend --api

made api folder in controllers, then subfolder v1

ran: rails g controller api/v1/articles index show create update destroy --skip-helper --skip-assets --skip-template-engine --skip-test-framework

rails g model article title:string body:string author:string --skip-helper --skip-assets --skip-template-engine --skip-test-framework

# will make new database to a SQLite DB 
rake db:create

rake db:migrate

bin/rails server

go to Postman

POST http://127.0.0.1:3000/api/v1/articles/

Body, raw, JSON

{
    "title": "new article",
    "body": "anything",
    "author": "name"
}

click Send button

GET request to same address

POST another

GET http://127.0.0.1:3000/api/v1/articles/1

this is to get by id

update article:

PUT http://127.0.0.1:3000/api/v1/articles/1

{

}

