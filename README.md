# Simple-React-App - Meetup

Install MongoDB Loopback Rest API

> npm install -g loopback-cli
> lb (to create the application)
> 3.x
> api-server
> node . (command to run the server)

-----------------
Browser: localhost:3000/explorer (loopback API explorer)

> npm install --save loopback-connector-mongodb (install loopback connector)
> lb datasource mongoDS --connector mongoDB

- Enter source name (Enter)
- Select  the connector for mongoDS 
    - MongoDB
- Connection String url (Skip)
- Host: localhost
- Port: 27017
- User: (Skip)
- Password: (Skip
- Database: meetupz-app

Create new model
> lb model

- model name: meetups
- select the datasource: db(mongodb)
- expose meetups via the rest api? y
- custom plural form: (skip)
- common model: common
- property name:
    - name
    - string
    - yes
    - (blank)

    - city
    - string
    - yes
    - blank

    - address
    - string
    - no
    - (blank)


> node .