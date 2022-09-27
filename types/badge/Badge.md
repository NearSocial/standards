# Badge

A Badge with the metadata and the list of the holders.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`info`** | [Badge Info](./Info.md) | The information describing the badge |
| **`holder`** | [Account List](../common/AccountList.md) | The list of the badge holders who were awarded with this badge |

## Example

```json
{
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
```

