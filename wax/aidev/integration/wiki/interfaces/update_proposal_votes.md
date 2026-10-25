[@hiveio/wax](../globals) / update\_proposal\_votes

# Interface: update\_proposal\_votes

A user may vote for proposals directly using an operation: update_proposal_votes_operation,
or indirectly using the proxy - operation:  account_witness_proxy_operation.
A user may vote for proposals submitted by the other users.
By voting for the proposal, a user may select which proposals should be funded.
A user may vote for as many proposals as they wants, but you cannot vote twice for the same proposal.
If a proxy is specified then all existing votes are deactivated. When the proxy is removed, the votes will be activated.
Your vote power depends on your HP.
If the operation account_witness_vote_operation or account_witness_proxy_operation or update_proposal_votes_operation
is not executed in HIVE_GOVERNANCE_VOTE_EXPIRATION_PERIOD, the votes are removed and the virtual operation:
expired_account_notification_operation is generated.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/45_update_proposal_votes.md?ref_type=heads

## Properties

### approve

> **approve**: `boolean`

#### Param

To vote for the proposal, the approve = true.
                        To remove the vote, the approve = false.

#### Defined in

wasm/lib/proto/update\_proposal\_votes.ts:29

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

#### Defined in

wasm/lib/proto/update\_proposal\_votes.ts:31

***

### proposal\_ids

> **proposal\_ids**: `string`[]

#### Param

IDs of proposals to vote for/against. Before HF28 nonexisting IDs are ignored from HF28 they trigger an error.

#### Defined in

wasm/lib/proto/update\_proposal\_votes.ts:24

***

### voter

> **voter**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/update\_proposal\_votes.ts:22
