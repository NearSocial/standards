# Root

Top level schema for an account

## Schema

| Key | Type | Description |
| --- | --- | --- |
| _`profile`_ | [Profile](./profile/Profile.md) | A profile information for the account |
| _`graph`_ | [Graph](./graph/Graph.md) | The outgoing graph connections from the account |
| _`badge`_ | [Badges](./badge/Badges.md) | Badges issued by the account and recipients of these badges |
| _`widget`_ | [Widgets](./widget/Widgets.md) | Widgets created by the account |
| _`post`_ | [Posts](./post/Posts.md) | Posts created by the account |
| _`settings`_ | [Settings](./settings/Settings.md) | Settings stored by the account |

## Example

```json
{
  "profile": {
    "name": "NEARCON 22 Demo Acc",
    "image": {
      "url": "https://cloudflare-ipfs.com/ipfs/QmQqzMTavQgT4f4T5v6PWBp7XNKtoPmC9jvn12WPT3gkSE"
    }
  },
  "graph": {
    "like": {
      "root.near": "",
      "mike.near": ""
    },
    "follow": {
      "mob.near": "",
      "root.near": ""
    }
  },
  "badge": {
    "whale": {
      "info": {
        "name": "Whale",
        "description": "A really whalethy user",
        "image": {
          "url": "https://upload.wikimedia.org/wikipedia/commons/e/e2/Southern_right_whale.jpg"
        }
      },
      "holder": {
        "x.near": "",
        "root.near": ""
      }
    }
  },
  "widget": {
    "HelloWorld": "return \"Hello World!\";",
    "Test": "return \"Test!\";"
  },
  "post": {
    "meme": {
      "title": "NEAR Protocol",
      "description": "Looks the same to me",
      "image": {
        "ipfs_cid": "bafkreicrp3nosvz4advbmp26dlmbjkl37gb7etztqf4gforuwxg5ofqov4"
      }
    }
  }
}
```
