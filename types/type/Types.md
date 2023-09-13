# Types

Types created by the account.

## Schema

| Key                  | Type                  | Description                                                  |
|----------------------|-----------------------|--------------------------------------------------------------|
| **`[type_name]`**  | [Type](./Type.md) | Contains the properties, references to widgets necessary to display and create data of this type, and the optional metadata. |

## Example

```json
{
  "Idea": {
    "": "{ \"properties\": [{\"name\": \"title\",\"type\": \"String\",\"required\": true }, {\"name\": \"description\",\"type\": \"md\",\"required\": false },], \"widgets\": {\"summary\": \"evrything.near/widget/Everything.Summary.Idea\",\"view\": \"evrything.near/widget/Everything.View.Idea\",\"create\": \"evrything.near/widget/Everything.Create.Idea\"}};",
    "metadata": {
      "name": "Idea",
      "description": "Idea type for proposals to the everything DAO",
      "tags": {
        "example": "",
        "inline": ""
      }
    }
  },
  "Event": {
    "": "{ \"properties\": [{\"name\": \"title\",\"type\": \"String\",\"required\": true }, {\"name\": \"description\",\"type\": \"md\",\"required\": false }, {\"name\": \"date\",\"type\": \"Date\",\"required\": true }], \"widgets\": {\"summary\": \"evrything.near/widget/Everything.Summary.Event\",\"view\": \"evrything.near/widget/Everything.View.Event\",\"create\": \"evrything.near/widget/Everything.Create.Event\"}};",
    "metadata": {
      "name": "Event",
      "description": "Event type for events approved by everything DAO",
      "tags": {
        "example": "",
        "inline": ""
      }
    }
  }
}
```
