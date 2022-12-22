# Bounty Claim

This exploratory standard is in DRAFT mode.

## Example

from the [Astro API](https://api.app.astrodao.com/docs/#/Bounty/BountyController_bountyById)

{
    "isArchived": true,
    "createdAt": "2022-12-22T04:35:37.608Z",
    "updatedAt": "2022-12-22T04:35:37.608Z",
    "transactionHash": "string",
    "updateTransactionHash": "string",
    "createTimestamp": "string",
    "updateTimestamp": "string",
    "id": "string",
    "accountId": "string",
    "startTime": "string",
    "deadline": "string",
    "completed": true,
    "endTime": "string"
}

___

from the Sputnik DAO [bounties.rs](https://github.com/near-daos/sputnik-dao-contract/blob/main/sputnikdao2/src/bounties.rs#L12-L21) file

pub struct BountyClaim {
  bounty_id: u64,
  start_time: U64,
  deadline: U64,
  completed: bool,
} 