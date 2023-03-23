# Type

Contains the properties, references to widgets necessary to display and create data of this type, and the optional metadata.

## Schema

| Key          | Type                              | Description                                     |
|--------------|-----------------------------------|-------------------------------------------------|
| **`""`**     | String                            | Schema describing the properities of a thing and holding references to necessary widgets for displaying and creating data of this type.                  |
| _`metadata`_ | [Metadata](../common/Metadata.md) | The metadata information describing the type. |

## Example

```json
{
  "": "{ \"properties\": [{\"name\": \"title\",\"type\": \"String\",\"required\": true }, {\"name\": \"description\",\"type\": \"md\",\"required\": false },], \"widgets\": {\"summary\": \"evrything.near/widget/Everything.Summary.Idea\",\"view\": \"evrything.near/widget/Everything.View.Idea\",\"create\": \"evrything.near/widget/Everything.Create.Idea\"}};",
  "metadata": {
    "name": "Idea",
    "description": "Idea type for proposals to the everything DAO",
    "tags": {
      "example": "",
      "inline": ""
    }
  }
}
```
