# Badge Info

The information for a badge.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`name`** | String(64) | The display name of the badge |
| **`description`** | String | The description for the badge |
| _`image`_ | [Image](../common/Image.md) | The display picture for the badge |

## Example

```json
{
  "name": "Whale",
  "description": "A really whalethy user",
  "image": {
    "url": "https://upload.wikimedia.org/wikipedia/commons/e/e2/Southern_right_whale.jpg"
  }
}
```
