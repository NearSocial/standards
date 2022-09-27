# Graph

The outgoing graph connections from the account.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[edge_type]`** | [Account List](../common/AccountList.md) | The key is the type of outgoing edges. For example, `follow` or `friend` edge types. |

## Example

```json
{
  "like": {
    "root.near": "",
    "mike.near": ""
  },
  "follow": {
    "mob.near": "",
    "root.near": ""
  }
}
```
