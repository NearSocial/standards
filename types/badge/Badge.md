# Badge

A Badge with the metadata and the list of the holders.

## Schema

| Key            | Type                                     | Description                                                                                 |
|----------------|------------------------------------------|---------------------------------------------------------------------------------------------|
| **`metadata`** | [Metadata](../common/Metadata.md)        | The metadata information describing the badge                                               |
| **`accounts`** | [Account List](../common/AccountList.md) | The list of the accounts that hold the given badge |

## Example

```json
{
  "metadata": {
    "name": "Whale",
    "description": "A really whalethy user",
    "image": {
      "url": "https://upload.wikimedia.org/wikipedia/commons/e/e2/Southern_right_whale.jpg"
    }
  },
  "accounts": {
    "x.near": "",
    "root.near": ""
  }
}
```

