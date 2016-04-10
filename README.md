# --------------Beczka Śpiewu-------------
## Get all songs
```http
GET /song
```
```json
{
  "len": 2,
  "songs": [
    {
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
      "list_id": "string",
      "content": "string",
      "chords_img_url": "string",
      "creationDate": "string"
    },
    {
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
      "list_id": "string",
      "content": "string",
      "chords_img_url": "string",
      "creationDate": "string"
    }
  ]
}
```
## Get one song
```http
GET /song/:id
```
```json
{
  "title": "string",
  "author": "string",
  "category": "string",
  "chords": "string",
  "list_id": "string",
  "content": "string",
  "chords_img_url": "string",
  "creationDate": "string"
}

```
## Get groups
```http
GET /group
```
```json
{
  "len": 2,
  "groups": [
    {
      "id": "string",
      "title": "string",
      "img_url": "string",
      "creationDate": "string"
    },
    {
      "id": "string",
      "title": "string",
      "img_url": "string",
      "creationDate": "string"
    }
  ]
}
```
## Get one group
```http
GET /group/:id
```
```json
{
  "id": "string",
  "title": "string",
  "img_url": "string",
  "creationDate": "string"
}
```
## Get lists
```http
GET /list
GET /list/group/:group_id
```
```json
{
  "len": 2,
  "lists":[
    {
      "id": "string",
      "group_id": "string",
      "title": "string",
      "img_url": "string",
      "songs": [
        {
          "title": "string",
          "author": "string",
          "category": "string",
          "chords": "string",
          "list_id": "string",
          "content": "string",
          "chords_img_url": "string"
        },
        {
          "title": "string",
          "author": "string",
          "category": "string",
          "chords": "string",
          "list_id": "string",
          "content": "string",
          "chords_img_url": "string"
        }]
    },
    {
      "id": "string",
      "group_id": "string",
      "title": "string",
      "img_url": "string",
      "songs": [
        {
          "title": "string",
          "author": "string",
          "category": "string",
          "chords": "string",
          "list_id": "string",
          "content": "string",
          "chords_img_url": "string"
        },
        {
          "title": "string",
          "author": "string",
          "category": "string",
          "chords": "string",
          "list_id": "string",
          "content": "string",
          "chords_img_url": "string"
        }]
    }
  ]
}
```
## Get one list
```http
GET /list/:id
```
```json
{
  "id": "string",
  "group_id": "string",
  "title": "string",
  "img_url": "string",
  "songs": [
    {
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
      "list_id": "string",
      "content": "string",
      "chords_img_url": "string"
    },
    {
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
      "list_id": "string",
      "content": "string",
      "chords_img_url": "string"
    }]
}
```
## Add song
```http
GET /song/add/?title=string&author=string&category=string&chords=string&list_id=string&chords_img_url=string&content=string
POST /song
```
```json
{
  "title": "string",
  "author": "string",
  "category": "string",
  "chords": "string",
  "list_id": "string",
  "content": "string",
  "chords_img_url": "string"
}
```
## Add list
```http
GET /list/add/?title=string&group_id=string&img_url=string
POST /list
```
```json
{
  "group_id": "string",
  "title": "string",
  "img_url": "string"
}
```
## Add group
```http
POST /group
```
```json
{
  "title": "string",
  "img_url": "string"
}
```
