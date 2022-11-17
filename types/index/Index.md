# Index

Index is a frequently overwritten object designed to be used by the API/indexer.
It should be used for actions associated with some key. For example: 
- for storing likes for a given post
- rating a certain item
- linking to a comment for a given post
- linking to a review for something

In order for the API server to index the data, it should be given in a specific format. Otherwise, the API server will ignore the data.

The format is `IndexData` which is a serialized JSON object with two keys: `key` and `data`.
- The `key` value will be used to index the data across all accounts. The API server will JSON serialize the value to create a unique string key for this index.
- The `data` value contains the data to be stored.
 
### Likes example

For example, an application want to store likes for a given post.
The post is identified by the following key: `mob.near/post/meme@76735731`. Then to create a like one may write the following IndexData (non-serialized):
```json
{
  "key": "mob.near/post/meme@76735731",
  "data": 1
}
```
This object will be serialized and should be added under `index/like`:
```json
{
  "index": {
    "like": "{\"key\":\"mob.near/post/meme@76735731\",\"data\":1}"
  }
}
```

The reason why we store this data in a serialized format is to be able to overwrite the previous data (that is already indexed) to reuse the storage.
The limitation of this approach is that only one action can be added per index per block. But since blocks are once a second, it shouldn't create issues.

An API server should be able to serve the following data:
- All likes for a given post from all users (or some users) ordered by block height when they were created.
- All likes for a given user ordered by block height.


## Schema

| Key | Type | Description                                                                                                                                  |
| --- | --- |----|
| **`[index_type]`** | Serialized IndexData (String) | The key is the type of index. For example, `like` or `comment`. The value is a serialized JSON object containing two fields `"key"` and `"data"` |

## Example

```json
{
  "like": "{\"key\":\"mob.near/post/meme@76735731\",\"data\":1}",
  "comment": "{\"key\":\"mob.near/post/meme@76735731\",\"data\":{\"type\":\"post/meme\"}}"
}
```
