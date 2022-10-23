# NFT

A pointer to an NFT. Contains a contract ID and a token ID.

## Schema

| Key | Type | Description |
| --- | --- | --- |
| _`contractId`_ | AccountID String(64) | An account ID of the NFT contract. |
| _`tokenId`_ | String | Token ID within the NFT contract. |

## Example

```json
{
  "contractId": "mrbrownproject.near",
  "tokenId": "3107"
}
```
