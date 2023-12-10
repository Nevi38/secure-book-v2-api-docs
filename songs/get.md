# API Songs

Returns a list of all songs of owner id.

**URL** : `/api/{owner}/songs`

**Method** : `GET`


## Parameters
**Required**

`owner`:  Owner id (ObjectId)

**Optional**

`limit`: The maximum number of songs to return. Default is 8.

`offset`: The number of songs to skip before starting to return results. Default is 0.

## Example
**Using Axios (JavaScript):**
```javascript
import axios from 'axios'

const owner = "653a17dbab118c7cf50002c5";
const endpoint = `http://localhost:3001/api/${owner}/songs?limit=2`;

(async function() {
  const response = await axios({
    method: 'get',
    url: endpoint
  });

  console.log(response.data)
})()
```

## Success Responses

**Code** : `200 OK`

**Content** : `JSON (Array)`

| Name          | Type    | Description                                         |
|-------------- |---------|-----------------------------------------------------|
| `_id`| ObjectId | Id song |
| `name`  | string  | Name of the song |
| `author`| string | Author of the song    |
| `path` | string  | Url to song.                           |
| `owner` | string  | Owner id (Song owner).      

```json
[
   {
        "_id": {
            "$oid": "6573d89382a3fd96a2f29d4d"
        },
        "name": "Điều cha chưa nói",
        "author": "Ali Hoàng Dương",
        "path": "1702090899889681117126.mp3",
        "owner": "653a17dbab118c7cf50002c5"
    },
    {
        "_id": {
            "$oid": "6573d89382a3fd96a2f29d4e"
        },
        "name": "River Flow In You",
        "author": "Yiruma",
        "path": "1702090899889681117123.mp3",
        "owner": "653a17dbab118c7cf50002c5"
    }  
]
```