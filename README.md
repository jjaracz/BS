# --------------Beczka Śpiewu-------------
## Get all songs
```http
GET /song
```
```json
{
  "songs": [
    {
      "id": "string",
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
      "creationDate": "string"
    },
    {
      "id": "string",
      "title": "string",
      "author": "string",
      "category": "string",
      "chords": "string",
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
  "id": "string",
  "title": "string",
  "author": "string",
  "category": "string",
  "chords": "string",
  "creationDate": "string"
}
```
## Get groups
```http
GET /group
```
```json
{
  "groups": [
    {
      "id": "string",
      "title": "string",
      "img": "url",
      "creationDate": "string"
    },
    {
      "id": "string",
      "title": "string",
      "img": "url",
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
  "img": "url",
  "creationDate": "string"
}
```
## Get lists
```http
GET /list
GET /list/:group_id
```
```json
{
  "lists": [
    {
      "id": "string",
      "title": "string",
      "group": "string"
    },
    {
      "id": "string",
      "title": "string",
      "group": "string"
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
  "title": "string",
  "group": "string",
  "img": "url"
}
```
## Add song
```http
GET /song/add/?title=string&author=string&category=string&chords=string
POST /song
```
```json
{
  "title": "string",
  "author": "string",
  "category": "string",
  "chords": "string"
}
```
## Add list
```http
GET /list/add/?title=string&group=string
POST /list
```
```json
{
  "title": "string",
  "group": "string",
  "img": "url"
}
```
## Add group
```http
POST /group
```
```json
{
  "title": "string",
  "img": "url"
}
```
