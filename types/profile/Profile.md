# Profile

Account's profile information.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`name`** | String(64) | The display name of the account |
| _`image`_ | [Image](../common/Image.md) | The profile picture |
| _`backgroundImage`_ | [Image](../common/Image.md) | The background image for the profile page |
| _`description`_ | Markdown(String) | The profile description in markdown format |
| _`linktree`_ | [LinkTree](code/standards/types/common/LinkTree.md) | A set of links for the profile |

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
  }
}
```
