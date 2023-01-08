# Bounty

This exploratory standard is in DRAFT mode.

## Schema

| Key | Type | About |
| --- | --- | --- |
| `bounty` | [Bounty](./Bounty.md) | bounty data |
| `bountyContext` | [BountyContext](./BountyContext.md) | about a bounty |
| `bountyClaims` | [BountyClaim](./BountyClaim.md) | self-assigned tasks |
| `bountyDoneProposals` | [BountyDoneProposal](./BountyDoneProposal.md) | payouts requested |
| `dao` | [Dao](./Dao.md) | reviewers / approvers |

## Example

The format used for storing a bounty.

{
  "id": "string",
  "bountyId": 0,
  "description": "string",
  "proposalId": "string",
  "daoId": "string",
  "dao": { ... },
  "bountyContext": { ... },
  "bountyDoneProposals": [ { ... } ]
  "bountyClaims": [ { ... } ]
  "description": "string",
  "token": "string",
  "amount": "string",
  "times": 0,
  "maxDeadline": "string",
  "numberOfClaims": 0
}


Astro API response for a given bounty ID:

https://api.app.astrodao.com/docs/#/Bounty/BountyController_bountyById


{
  "isArchived": true,
  "createdAt": "2022-12-22T04:35:37.607Z",
  "updatedAt": "2022-12-22T04:35:37.607Z",
  "transactionHash": "string",
  "updateTransactionHash": "string",
  "createTimestamp": "string",
  "updateTimestamp": "string",
  "id": "string",
  "bountyId": 0,
  "proposalId": "string",
  "daoId": "string",
  "dao": { ... },
  "bountyContext": { ... },
  "bountyDoneProposals": [{ ... }]
  "bountyClaims": [{ ... }],
  "description": "string",
  "token": "string",
  "amount": "string",
  "times": 0,
  "maxDeadline": "string",
  "numberOfClaims": 0
}