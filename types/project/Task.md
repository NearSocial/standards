# Task

A `Task` is work that needs to be done for a `Project`.

This standard is in DRAFT mode. It may be heavily changed in the future.

## Schema

| Key | Type | Description |
|---------------------|----------------------|-----------------------------------------------------------------------|
| `metadata` | [Metadata](../common/Metadata.md) | info describing a task |
| `token` | String | key is the ID of a token used as reward for the task |
| `amount` | String | key is the amount of tokens paid to the worker |
| `worker` | String | key is the account ID of someone who claims the task |

## Example

```json
{
    "metadata": {
        "name": "TODO",
        "description": "Create ...",
        "tags": {
          "design": "",
          "art": "",
          "community": ""
        }
    },
    "token": "meta-token.near",
    "amount": "888",
    "worker": "devs.near"
}
```