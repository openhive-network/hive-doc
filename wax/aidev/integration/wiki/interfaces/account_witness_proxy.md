[@hiveio/wax](../globals) / account\_witness\_proxy

# Interface: account\_witness\_proxy

A user may vote for a witness or proposal directly (using an operation: account_witness_vote_operation or update_proposal_votes_operation)
or indirectly (using the proxy - operation:  account_witness_proxy_operation).
If a user sets a proxy, the witness votes are removed and the proposal votes are deactivated.
If a user removes a proxy, there are no witness votes and the proposal votes are activated.
Settings proxy means that a user wants to cede a decision on which witnesses to vote for to an account indicated as {proxy}.
{proxy} will also vote for proposals in the name of {account}.
If the operation account_witness_vote_operation or account_witness_proxy_operation or update_proposal_votes_operation is not executed
in HIVE_GOVERNANCE_VOTE_EXPIRATION_PERIOD, the votes are removed and the virtual operation:
expired_account_notification_operation is generated.
If the proxy was set and now it is removed, the additionally the virtual operation: proxy_cleared_operation is generated.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/13_account_witness_proxy.md?ref_type=heads

## Properties

### account

> **account**: `string`

#### Param

#### Defined in

wasm/lib/proto/account\_witness\_proxy.ts:21

***

### proxy

> **proxy**: `string`

#### Param

Account name. To remove the proxy, the parameter should be set empty.
                        Only one proxy may be set for an account.

#### Defined in

wasm/lib/proto/account\_witness\_proxy.ts:26
