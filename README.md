# --------------Beczka Śpiewu-------------
## Get all songs
```http
GET /song
```
```json
{
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
SONG{
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
  "lists": [
    {
      "id": "string",
      "group_id": "string",
      "title": "string",
      "img_url": "string"
    },
    {
      "id": "string",
      "group_id": "string",
      "title": "string",
      "img_url": "string"
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
  "img_url": "string"
}
```
## Add song
```http
GET /song/add/?title=string&author=string&category=string&chords=string&list=id
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
  "chords_img_url": "string",
  "creationDate": "string"
}
```
## Add list
```http
GET /list/add/?title=string&group=id&img=url
POST /list
```
```json
{
  "id": "string",
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
  "id": "string",
  "title": "string",
  "img_url": "string",
  "creationDate": "string"
}
```
