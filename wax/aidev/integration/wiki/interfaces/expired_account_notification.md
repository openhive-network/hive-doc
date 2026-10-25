[@hiveio/wax](../globals) / expired\_account\_notification

# Interface: expired\_account\_notification

Related to governance voting: account_witness_vote_operation, account_witness_proxy_operation and update_proposal_votes_operation.
Generated during block processing when user did not cast any governance vote for very long time. Such user is considered not
interested in governance and therefore his previous votes are nullified.

## Properties

### account

> **account**: `string`

#### Param

user whose governance votes were nullified

#### Defined in

wasm/lib/proto/expired\_account\_notification.ts:12
