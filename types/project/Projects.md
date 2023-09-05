# Projects

`Projects` with `metadata`, `editors`, and `tasks`.

This standard is in DRAFT mode. It may be heavily changed in the future.

## Schema

| Key | Type | Description |
|---------------------|----------------------|-----------------------------------------------------------------------|
| `[project_name]` | [Project](./Project.md) | key is the name of a project, for example: `near_social` |

## Example

```json
{
  "near_social": {
    "metadata": {
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
        "description": "Near Social is ...",
        "backgroundImage": {
            "ipfs_cid": "bafybeigwqqx2eccpyip66bn2bn6janvss2snv3xuuus3ltin6i46mfkyam"
        },
        "tags": {
            "project": "",
            "near-social": "",
            "open-source": ""
        }
    },
    "editors": {
        "root.near": "",
        "mob.near": "",
        "infinity.near": ""
    },
    "tasks": {
        "task_1": {
            "metadata": {
                "name": "Task 1",
                "description": "Create ABC",
                "tags": {
                    "design": "",
                    "art": "",
                    "community": ""
                }
            },
            "token": "token.paras.near",
            "amount": "359",
            "worker": "create.near"
        },
        "task_2": {
            "metadata": {
                "name": "Task 2",
                "description": "Create XYZ",
                "tags": {
                    "dev": "",
                    "product": "",
                    "javascript": ""
                }
            },
            "token": "meta-token.near",
            "amount": "888",
            "worker": "devs.near",
        }
    }
  }
}
```