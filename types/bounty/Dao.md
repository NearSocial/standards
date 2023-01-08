# DAO

This exploratory standard is in DRAFT mode.

## Schema

from [DAOstar](https://daostar.org/schema)

| Type | About |
| --- | --- |
| name | title of the DAO |
| description | info regarding the DAO |
| membersURI | pointing to a Json file representing the Members object |
| proposalsURI | pointing to a Json file representing the Proposals object |
| activityLogURI | pointing to a Json file representing the Activity Log object |
| governanceURI | pointing to a flat file, detailing the governance system of the DAO |

## Example

from the [Astro API](https://api.app.astrodao.com/docs/#/DAO/DaoController_daoById)

{
    "isArchived": true,
    "createdAt": "string($date-time)",
    "updatedAt": "string($date-time)",
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
        "createdAt": "string($date-time)",
        "updatedAt": "string($date-time)",
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
            "createdAt": "string($date-time)",
            "updatedAt": "string($date-time)",
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
        "createdAt": "2022-12-22T04:35:37.608Z",
        "updatedAt": "2022-12-22T04:35:37.608Z",
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
}

___

## Common Interfaces for DAOs

from [EIP-4824](https://eips.ethereum.org/EIPS/eip-4824), courtesy of [DAOstar](https://daostar.one)

{
    "@context": "http://www.daostar.org/schemas",
    "type": "DAO",
    "name": "<name of the DAO>",
    "description": "<description>",
    "membersURI": "<URI>",
    "proposalsURI": "<URI>",
    "activityLogURI": "<URI>",
    "governanceURI": "<URI>",
		"contractsRegistryURI": "<URI>"
}

### Members

{
    "@context": "<http://www.daostar.org/schemas>",
    "type": "DAO",
    "name": "<name of the DAO>",
    "members": [
        {
            "type": "EthereumAddress",
            "id": "<address or other identifier>"
        },
        {
            "type": "EthereumAddress",
            "id": "<address or other identifier>"
        }
    ]
}

### Proposals

{
    "@context": "http://www.daostar.org/schemas",
    "type": "DAO",
    "name": "<name of the DAO>",
    "proposals": [
        {
            "type": "proposal",
            "id": "<proposal ID>",
            "name": "<name or title of proposal>",
            "contentURI": "<URI to content or discussion>",
            "status": "<status of proposal>",
            "calls": [
                {
                    "type": "CallDataEVM",
                    "operation": "<call or delegate call>",
                    "from": "<EthereumAddress>",
                    "to": "<EthereumAddress>",
                    "value": "<value>",
                    "data": "<call data>"
                }
            ]
        }
    ]
}

### Contracts Registry

{
    "@context": "<http://www.daostar.org/schemas>",
    "type": "DAO",
    "name": "<name of the DAO>",
    "contracts": [
        {
            "type": "EthereumAddress",
            "id": "<address or other identifier>",
						"label": "Treasury"
        },
        {
            "type": "EthereumAddress",
            "id": "<address or other identifier>",
						"label": "Governance Token"

        }
    ]
}

### Activity Log

{
    "@context": "<http://www.daostar.org/schemas>",
    "type": "DAO",
    "name": "<name of the DAO>",
    "activities": [
        {
            "id": "<activity ID>",
            "type": "activity",
            "proposal": {
                "id": "<proposal ID>",
                "type": "proposal"
            },
            "member": {
                "type": "EthereumAddress",
                "id": "<address or other identifier>"
            }
        }, 
    "activities": [
        {
            "id": "<activity ID>",
            "type": "activity",
            "proposal": {
                "id": "<proposal ID>",
                "type": "proposal"
            },
            "member": {
                "type": "EthereumAddress",
                "id": "<address or other identifier>"
            }
        }
    ]
}