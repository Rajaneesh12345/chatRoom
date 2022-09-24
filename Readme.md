# # ChatApp

## Features

-   Join a specified room to chat
    
-   Send the geographical location to other users in the room if permission is granted
    
-   Automatically scroll down upon receiving a new message
    
-   Responsive web design (RWD)


## [](https://github.com/rubychi/udemy-chatapp#getting-started)Getting Started

Follow the instructions below to set up the environment and run this project on your local machine

### [](https://github.com/rubychi/udemy-chatapp#prerequisites)Prerequisites

-   Node.js

### [](https://github.com/rubychi/udemy-chatapp#installing)Installing

1.  Download ZIP or clone this repo

```
> git clone https://github.com/Rajaneesh12345/chatRoom.git
```

2.  Install dependencies via NPM

```
> npm install
```

3. Create a config.json to securely store credentials inside \server\config

```
{
  "test": {
    "PORT": "3000",
    "MONGODB_URI": "mongodb://localhost:27017/APPNAME1"
  },
  "development": {
    "PORT": "3000",
    "MONGODB_URI": "mongodb://localhost:27017/APPNAME2"
  }
}
```

4.  Back to the root directory and type the below command to start the server and the service

```
> npm run dev-watch
```

5.  See it up and running on  [http://localhost:3000](http://localhost:3000/)

## [](https://github.com/rubychi/udemy-chatapp#deployment)Deployment

1.  Deploy to Heroku

```
> heroku create
> git push heroku master
```

2. Set up config variables

```
> heroku config:set
  MONGODB_URI=[Your MongoDB URI]
```

3.  Open the app in the browser

```
> heroku open
```



## [](https://github.com/rubychi/udemy-chatapp#built-with)Built With

### [](https://github.com/rubychi/udemy-chatapp#frontend)Frontend

-   jquery
-   mustache

### [](https://github.com/rubychi/udemy-chatapp#backend)Backend

-   express
-  NodeJS
-   compression
-   helmet

### [](https://github.com/rubychi/udemy-chatapp#utils)Utils

-   socket.io
-   moment


##  Notes

-   Send an event to everybody in the room 'The Office Fans'

```
io.emit -> io.to('The Office Fans').emit

```

-   Send an event to everybody in the room 'The Office Fans' except for the current user

```
socket.broadcast.emit -> socket.broadcast.to('The Office Fans').emit

```

-   Send an event to a specific user

```
socket.emit
```

## Authors

- [Rajaneesh Gudivada](https://github.com/Rajaneesh12345)