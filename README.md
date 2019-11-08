## Basic-JSON-Server
how to create a basic json server and how to use it with rest API.  

## 1. Install JSON Server
`npm install -g json-server`.

## 2. Create Server file
Create a `db.json` file. (your preferred name but .json is compulsory)
and enter some data in json format.
```
 {
  "posts": [
    { "id": 1, "title": "Name 1" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```

## 3. Start JSON Server
`json-server --watch db.json` (fileName.json)

## 4. Connect
  http://localhost:3000/<br>
  http://localhost:3000/nameList/<br>
  http://localhost:3000/nameList/1<br>

if you go to http://localhost:3000/nameList/1, you'll get<br>

{ "id": 1, "title": "Name 1" }
