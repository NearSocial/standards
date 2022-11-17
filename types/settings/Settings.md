# Settings [DRAFT]

Settings stored by the account. 

This standard is in DRAFT mode. It may be heavily changed in the future.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[project_identifier]`** | [KeyValue](../common/KeyValue.md) | The key is a project identifier. For example, `near.social`, `wallet.near.org`, `SuperMessenger` all can be identifiers. |

## Example

```json
{
  "near.social": {
    "homepage": "mob.near/widget/Welcome"
  }
}
```
