# Widget

Contains the source code and the optional metadata.

## Schema

| Key          | Type                              | Description                                     |
|--------------|-----------------------------------|-------------------------------------------------|
| **`""`**     | String                            | The source code of the widget.                  |
| _`metadata`_ | [Metadata](../common/Metadata.md) | The metadata information describing the widget. |

## Example

```json
{
  "": "return \"Hello World!\";",
  "metadata": {
    "name": "Hello World",
    "description": "Renders Hello World",
    "tags": {
      "example": "",
      "inline": ""
    }
  }
}
```

