# Easy-JSON-server

# Author: Keaton Gallagher

## Description
  This is a easy fake JSON server you can run locally and create your own data to test without having to create a DB.

## Getting Started 
  1. Create directory:  mkdir name-of-file
  2. Enter into directory: cd name-of-file
  3. Install package: sudo npm install -g json-server or sudo yarn install -g json-server
  4.Create db.json file and add the json you want EX:

```
  {
    "friends": [
      {
        "id": 1,
        "first_name": "tommy",
        "last_name": "John",
        "email": "tester@thetest.com"
      },
      {
        "id": 2,
        "first_name": "Rob",
        "last_name": "Swanson",
        "email": "Rob@Swanson.com"
      },
      {
        "id": 3,
        "first_name": "Laura",
        "last_name": "Gene",
        "email": "Gene@kgallagher.com"
      }
    ]
  }

```

5.Run the server: json-server --watch db.json

6. EndPoints: 

```
  GET    /friends
  GET    /friends/{id}
  POST   /friends
  PUT    /friends/{id}
  PATCH  /friends/{id}
  DELETE /friends/{id}

```

7. Hitting EndPoints:

```
  http://localhost:3000/friends?first_name=Laura
  http://localhost:3000/friends?q=kgallagher
  You can also use postman
  localhost:3000/friends/

```
### Extra Resources

  1. Changing port: json-server -p 4000 db.json