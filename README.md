# Secure Book V2 API

<style>
    .flex {
        display: flex; 
    }

    .align-items-center {
        align-items: center;
    }

    .justify-content-center {
        justify-content: center;
    }

    .flex-column {
        flex-direction: column;
    }
    
    .flex img {
        margin-right: 10px;
    }

    .deny {
        color: red;
    }

    .allow {
        color: green;
    }
</style>

<div class="flex justify-content-center">
<img style="border-radius: 50%; width: 200px; height: 200px" src="https://www.vietnamfineart.com.vn/wp-content/uploads/2023/03/hinh-anh-co-gai-cute-anime-8-min-4.jpg">
<img style="border-radius: 50%; width: 200px; height: 200px" src="https://tranhdecors.com/wp-content/uploads/edd/2023/09/Hinh-nen-Anime-nu-hoang-mat-xanh-biec.jpg">
<img style="border-radius: 50%; width: 200px; height: 200px" src="https://i.pinimg.com/originals/d7/80/75/d78075041fedd4813f0462433d15ebd8.jpg">
</div>

### HTTP method
- `GET`: Retrieving resources.
- `POST`: Creating resources.
- `DELETE`: Deleting resources.
- `PUT`: Replacing resources or collections of resources.

<br>

<div class="flex">
    <img style="border-radius: 50%; width: 50px; height: 50px" src="https://top10tphcm.com/wp-content/uploads/2023/06/anh-anime-buon-nu.jpg">
    <div class="flex flex-column">
        <b>Song API</b>
        <p>Endpoints for viewing and manipulating Songs.</p>
    </div>
</div>

|Method|Endpoint|Tutorial|Allow|
|------|---------|-------|-----|
<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">GET</span>|/api/{owner}/songs|[Get all songs](songs/get.md)| <span class="allow">Yes</span> |
|<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">POST</span>|/api/{owner}/songs/{song}|[Add song](songs/post.md)|<span class="deny">No</span>|
|<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: red; border-radius: 20px;">DELETE</span>|/api/{owner}/songs/{song}|[Delete an song](songs/delete.md)|<span class="allow">Yes</span>|
<span style="font-size: 12px ;display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">PUT</span>|/api/{owner}/songs/{song}|[Edit an song](songs/put.md)| <span class="allow">Yes</span> |

<br>

<div class="flex">
    <img style="border-radius: 50%; width: 50px; height: 50px" src="https://i.pinimg.com/originals/d7/80/75/d78075041fedd4813f0462433d15ebd8.jpg">
    <div class="flex flex-column">
        <b>Account API</b>
        <p>Endpoints for viewing and manipulating the Account</p>
    </div>
</div>

| Method | Endpoint                | Tutorial                              | Allow |
|--------|-------------------------|---------------------------------------|-------|
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">POST</span> | /api/account | [Create an account](account/post.md) | <span class="allow" style="color: green;">Yes</span> |

<br>

<div class="flex">
    <img style="border-radius: 50%; width: 50px; height: 50px" src="https://i.pinimg.com/originals/d7/80/75/d78075041fedd4813f0462433d15ebd8.jpg">
    <div class="flex flex-column">
        <b>Friend API</b>
        <p>Endpoints for viewing and manipulating the Account</p>
    </div>
</div>

| Method | Endpoint                  | Tutorial                              | Allow |
|--------|---------------------------|---------------------------------------|-------|
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">GET</span> | /api/friends | [Get Friends](friends/get.md)    | <span class="allow" style="color: green;">Yes</span> |
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: #0967d5; border-radius: 20px;">POST</span> | /api/friends | [Add a Friend](friends/post.md) | <span class="allow">Yes</span> |
| <span style="font-size: 12px; display: inline-block; color: white; padding: 0 10px; background-color: red; border-radius: 20px;">DELETE</span> | /api/friends/{friendId} | [Remove a Friend](friends/delete.md) | <span class="allow">Yes</span> |

## Author by Nevi38
![ending](https://top10tphcm.com/wp-content/uploads/2023/06/anh-anime-buon-nu.jpg "ss")