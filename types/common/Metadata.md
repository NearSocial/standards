# Metadata

Generic metadata object describing an entity.

## Schema

| Key                 | Type                      | Description                            |
|---------------------|---------------------------|----------------------------------------|
| **`name`**          | String(64)                | The display name or title              |
| _`image`_           | [Image](./Image.md)       | The main image or an icon              |
| _`backgroundImage`_ | [Image](./Image.md)       | The background image                   |
| _`description`_     | Markdown(String)          | The description in the markdown format |
| _`linktree`_        | [LinkTree](./LinkTree.md) | Links                                  |
| _`tags`_            | [Tags](./Tags.md)         | Tags                                   |


## Example

```json
{
  "name": "Near Social",
  "image": {
    "ipfs_cid": "bafkreid55mbassw335wezjk3gc5rzizwrqpenfxk3dyyljumxvezplhjg4"
  },
  "linktree": {
    "twitter": "NearSocial_",
    "github": "NearSocial",
    "telegram": "NearSocial",
    "website": "near.social"
  },
  "description": "# Near Social\n\n**Near Social** is ...",
  "backgroundImage": {
    "ipfs_cid": "bafybeigwqqx2eccpyip66bn2bn6janvss2snv3xuuus3ltin6i46mfkyam"
  },
  "tags": {
    "platform": "",
    "project": "",
    "network": "",
    "protocol": "",
    "open-source": ""
  }
}
```
