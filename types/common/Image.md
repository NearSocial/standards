# Image

A common image.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| _`url`_ | URL String | A direct URL to the image source. |
| _`ipfs_cid`_ | CID String | IPFS CID to the image. |
| _`nft`_ | [NFT](./NFT.md) | Pointer to an NFT. |

At least one the keys is required. Ideally, you should provide exactly one of the keys, but it's not strictly required.
The image should be displayed in the following priority order:
1. `nft`
1. `ipfs_cid`
1. `url`

## Example

```json
{
  "img": "https://cloudflare-ipfs.com/ipfs/QmQqzMTavQgT4f4T5v6PWBp7XNKtoPmC9jvn12WPT3gkSE"
}
```

```json
{
  "ipfs_cid": "bafkreigfsxev7mc6hkdc55ey6hx4zmbrhipsvy32vwn45vw6zbg2hgzugu"
}
```

```json
{
  "nft": {
    "contractId": "mrbrownproject.near",
    "tokenId": "3107"
  }
}
```
