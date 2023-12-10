# Secure Book V2 API

<img src="https://tranhdecors.com/wp-content/uploads/edd/2023/09/Hinh-nen-Anime-nu-hoang-mat-xanh-biec.jpg">


### HTTP method
- `GET`: Retrieving resources.
- `POST`: Creating resources.
- `DELETE`: Deleting resources.
- `PUT`: Replacing resources or collections of resources.

### Song API
Endpoints for viewing and manipulating Songs.

|Method|Endpoint|Tutorial|Allow|
|------|---------|-------|-----|
<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">GET</span>|/api/{owner}/songs|[Get all songs](songs/get.md)| <span style="color: green">Yes</span> |
|<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">POST</span>|/api/{owner}/songs/{song}|[Add song](songs/post.md)|<span style="color: red">No</span>|
|<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: red; border-radius: 20px;">DELETE</span>|/api/{owner}/songs/{song}|[Delete an song](songs/delete.md)|<span style="color: green">Yes</span>|
<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">PUT</span>|/api/{owner}/songs/{song}|[Edit an song](songs/put.md)| <span style="color: green">Yes</span> |


### Account API
Endpoints for viewing and manipulating the Account

| Method | Endpoint                | Tutorial                              | Allow |
|--------|-------------------------|---------------------------------------|-------|
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">POST</span> | /api/account | [Create an account](account/post.md) | <span style="color: green;">Yes</span> |


### Comment API
Endpoints for viewing and manipulating the Comment

| Method | Endpoint                     | Tutorial                                | Allow |
|--------|------------------------------|-----------------------------------------|-------|
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">GET</span> | /api/comments/{owner}         | [Get Comments](comments/get.md)         | <span style="color: green;">Yes</span>  |
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">GET</span> | /api/comments/{commentId}         | [Get details a comment](comments/get-by-id.md)         | <span style="color: green;">Yes</span>  |