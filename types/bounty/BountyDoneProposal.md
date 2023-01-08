# Bounty Proposal

This exploratory standard is in DRAFT mode.

## Example

The format used for storing a "bounty done" proposal.

{
      "isArchived": true,
      "createdAt": "string($date-time)",
      "updatedAt": "string($date-time)",
      "transactionHash": "string",
      "updateTransactionHash": "string",
      "createTimestamp": "string",
      "updateTimestamp": "string",
      "id": "string",
      "proposalId": 0,
      "daoId": "string",
      "dao": {
       
      "proposer": "string",
      "description": "string",
      "status": "InProgress",
      "voteStatus": "Active",
      "kind": {
        "type": "ChangeConfig",
        "config": {
          "name": "string",
          "purpose": "string",
          "metadata": "string"
        },
        "policy": {
          "proposalBond": "string",
          "bountyBond": "string",
          "proposalPeriod": "string",
          "bountyForgivenessPeriod": "string",
          "defaultVotePolicy": {
            "weightKind": "TokenWeight",
            "quorum": "string",
            "kind": "Weight",
            "weight": "string",
            "ratio": [
              "string"
            ]
          },
          "roles": {
            "id": "string",
            "name": "string",
            "balance": 0,
            "accountIds": [
              "string"
            ],
            "permissions": [
              "string"
            ],
            "votePolicy": {},
            "kind": {
              "group": [
                "string"
              ]
            }
          }
        },
        "proposalVariant": "string",
        "memberId": "string",
        "role": "string",
        "receiverId": "string",
        "actions": [
          {
            "methodName": 0,
            "args": "string",
            "deposit": "string",
            "gas": "string"
          }
        ],
        "hash": "string",
        "methodName": "string",
        "tokenId": "string",
        "msg": "string",
        "stakingId": "string",
        "bounty": "string",
        "bountyId": 0,
        "amount": "string"
      },
      "type": "ChangeConfig",
      "submissionTime": "string",
      "voteCounts": {},
      "votes": {},
      "failure": {},
      "actions": [
        {
          "id": "string",
          "proposalId": "string",
          "accountId": "string",
          "action": {},
          "transactionHash": "string",
          "timestamp": "string"
        }
      ],
      "votePeriodEnd": "string",
      "bountyDoneId": "string",
      "bountyClaimId": "string",
      "commentsCount": 0,
      "permissions": {
        "canApprove": true,
        "canReject": true,
        "canDelete": true,
        "isCouncil": true,
        "canAdd": true
      }
    }
}

___

from the Sputnik DAO [proposals.rs](https://github.com/near-daos/sputnik-dao-contract/blob/main/sputnikdao2/src/proposals.rs) file:

pub struct PolicyParameters {
    pub proposal_bond: Option<U128>,
    pub proposal_period: Option<U64>,
    pub bounty_bond: Option<U128>,
    pub bounty_forgiveness_period: Option<U64>,
}

AddBounty { bounty: Bounty },

BountyDone {
    bounty_id: u64,
    receiver_id: AccountId,
},