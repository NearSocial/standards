# Tasks

`Tasks` with metadata, token rewards, and a worker.

This standard is in DRAFT mode. It may be heavily changed in the future.

## Schema

| Key | Type | Description |
|---------------------|----------------------|-----------------------------------------------------------------------|
| `[task_id]` | [Task](./Task.md) | key is the ID / name of a task |

## Example

```json
{
  "example_task": {
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
}
```