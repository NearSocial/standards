# Bounty Context

This exploratory standard is in DRAFT mode.

## Example

The format used for storing the bounty metadata.

{
    "isArchived": true,
    "createdAt": "2022-12-22T04:35:37.607Z",
    "updatedAt": "2022-12-22T04:35:37.607Z",
    "id": "string",
    "daoId": "string",
    "proposal": {
      "isArchived": true,
      "createdAt": "2022-12-22T04:35:37.607Z",
      "updatedAt": "2022-12-22T04:35:37.607Z",
      "transactionHash": "string",
      "updateTransactionHash": "string",
      "createTimestamp": "string",
      "updateTimestamp": "string",
      "id": "string",
      "proposalId": 0,
      "daoId": "string",
      "dao": {
        "isArchived": true,
        "createdAt": "2022-12-22T04:35:37.607Z",
        "updatedAt": "2022-12-22T04:35:37.607Z",
        "transactionHash": "string",
        "updateTransactionHash": "string",
        "createTimestamp": "string",
        "updateTimestamp": "string",
        "id": "string",
        "config": {
          "name": "string",
          "purpose": "string",
          "metadata": "string"
        },
        "metadata": {},
        "amount": "string",
        "totalSupply": "string",
        "lastBountyId": 0,
        "lastProposalId": 0,
        "stakingContract": "string",
        "numberOfAssociates": 0,
        "numberOfMembers": 0,
        "numberOfGroups": 0,
        "council": [
          "string"
        ],
        "accountIds": [
          "string"
        ],
        "councilSeats": 0,
        "policy": {
          "isArchived": true,
          "createdAt": "2022-12-22T04:35:37.607Z",
          "updatedAt": "2022-12-22T04:35:37.607Z",
          "daoId": "string",
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
          "roles": [
            {
              "isArchived": true,
              "createdAt": "2022-12-22T04:35:37.607Z",
              "updatedAt": "2022-12-22T04:35:37.607Z",
              "id": "string",
              "name": "string",
              "kind": "string",
              "balance": 0,
              "accountIds": [
                "string"
              ],
              "permissions": [
                "string"
              ],
              "votePolicy": {
                "additionalProp1": {
                  "weightKind": "TokenWeight",
                  "quorum": "string",
                  "kind": "Weight",
                  "weight": "string",
                  "ratio": [
                    "string"
                  ]
                },
                "additionalProp2": {
                  "weightKind": "TokenWeight",
                  "quorum": "string",
                  "kind": "Weight",
                  "weight": "string",
                  "ratio": [
                    "string"
                  ]
                },
                "additionalProp3": {
                  "weightKind": "TokenWeight",
                  "quorum": "string",
                  "kind": "Weight",
                  "weight": "string",
                  "ratio": [
                    "string"
                  ]
                }
              }
            }
          ]
        },
        "createdBy": "string",
        "daoVersionHash": "string",
        "daoVersion": {
          "isArchived": true,
          "createdAt": "2022-12-22T04:35:37.607Z",
          "updatedAt": "2022-12-22T04:35:37.607Z",
          "hash": "string",
          "version": [
            "string"
          ],
          "commitId": "string",
          "changelogUrl": "string"
        },
        "status": {},
        "activeProposalCount": 0,
        "totalProposalCount": 0,
        "totalDaoFunds": 0,
        "bountyCount": 0,
        "nftCount": 0
      },
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
    },
    "bounty": "string",
    "commentsCount": 0
  },