# Account List

A list of account IDs. For example, receivers of a badge or a list of accounts you follow.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[account_id]`** | Empty string | A dynamic key representing the account ID for every account in the list. For example, `alex.near` as a key means that the account `alex.near` belongs to the list. |

## Example

```json
{
  "alex.near": "",
  "root.near": "",
  "mike.near": ""
}
```
