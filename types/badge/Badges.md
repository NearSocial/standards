# Badges

Badges issued by the account and holders for each of these badges.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[badge_name]`** | [Badge](./Badge.md) | The key is the name of a badge. For example, `whale` or `real_human`. |

## Example

```json
{
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
}
```
