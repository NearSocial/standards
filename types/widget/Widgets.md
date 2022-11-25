# Widgets

Widgets created by the account.

## Schema

| Key | Type   | Description |
| --- |--------| --- |
| **`[widget_name]`** | Widget | The source code of the widget with the given `widget_name`. The widget name should be in CamelCase, e.g. `MyExampleWidget`. |

## Example

```json
{
  "HelloWorld": "return \"Hello World!\";",
  "Test": "return \"Test!\";"
}
```
