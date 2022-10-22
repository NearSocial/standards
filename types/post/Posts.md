# Posts [DRAFT]

Posts/updates creates by the account. The intention of the posts is to be displayed in a social media networks.
The posts should be overwritten when a new post of the same type is added.
Using blockchain history the whole post history can be recovered and displayed.

This standard is in DRAFT mode. It may be heavily changed in the future.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[post_type]`** | [Post](./Post.md) | The key is the type of a post. For example, `meme`, `status`, `update` types. |

## Example

```json
{
  "meme": {
    "title": "NEAR Protocol",
    "description": "Looks the same to me",
    "image": {
      "ipfs_cid": "bafkreicrp3nosvz4advbmp26dlmbjkl37gb7etztqf4gforuwxg5ofqov4"
    }
  },
  "status": {
    "message": "Hello world!"
  }
}
```
