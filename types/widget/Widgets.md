# Widgets

Widgets created by the account.

## Schema

| Key                  | Type                  | Description                                                  |
|----------------------|-----------------------|--------------------------------------------------------------|
| **`[widget_name]`**  | [Widget](./Widget.md) | Contains the source code and the optional metadata |

## Example

```json
{
  "HelloWorld": {
    "": "return \"Hello World!\";",
    "metadata": {
      "name": "Hello World",
      "description": "Renders Hello World",
      "tags": {
        "example": "",
        "inline": ""
      }
    }
  },
  "Test": "return \"Test!\";"
}
```
