# LinkTree

Account's linktree information.

### Known providers

Key is the `link_name`. The value contains the prefix and the icon.

```
const linktreeElements = {
  website: {
    prefix: "https://",
    icon: "bi-globe2",
  },
  github: {
    prefix: "https://github.com/",
    icon: "bi-github",
  },
  twitter: {
    prefix: "https://twitter.com/",
    icon: "bi-twitter",
  },
  telegram: {
    prefix: "https://t.me/",
    icon: "bi-telegram",
  },
};
```

## Schema

| Key | Type | Description |
| --- | --- | --- |
| **`[link_name]`** | String | The link for the given `link_name`. The value doesn't have to be a full URL for known providers described in this doc. |

## Example

```json
{
  "twitter": "NearSocial_",
  "github": "NearSocial",
  "telegram": "NearSocial",
  "website": "near.social"
}
``` 
