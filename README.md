# --------------Beczka Śpiewu-------------
## Get all songs
```http
GET /songs
```
```json
{
  "title": "string",
  "author": "string",
  "category": "string",
  "chords": "string",
  "creationDate": "string"
}
```
## Get one song
```http
GET /songs/:id
```
## Get groups
```http
GET /group
```
```json
{
  "groups": [
    {
      "title": "string",
      "img": "url",
      "creationDate": "string"
    },
    {
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
GET /lists
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
  "group": "string"
}
```
## Add song
```http
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
```http
GET /song/add/?title=string&author=string&category=string&chords=string
```
## Add list
```http
GET /list/add/?title=string&group=string
POST /list
```
```json
{
  "title": "string",
  "category": "string",
  "group": "string"
}
```
## Add group
```http
POST /group
```
```json
{
  "title": "string",
  "category": "string",
  "img": "url"
}
```
