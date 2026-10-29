[@hiveio/wax](../globals) / account\_witness\_vote

# Interface: account\_witness\_vote

Defined in: wasm/lib/proto/account\_witness\_vote.ts:18

A user may vote for a witness directly using an operation:
account_witness_vote_operation or indirectly using the proxy - operation:  account_witness_proxy_operation.
All accounts with a Hive Power (also called Vesting Fund Shares or VESTS) can vote for up to 30 witnesses,
but you cannot vote twice for the same witnesses.
If a proxy is specified then all existing votes are removed.
Your vote power depends on your HP.
If the operation account_witness_vote_operation or account_witness_proxy_operation or update_proposal_votes_operation
is not executed in a HIVE_GOVERNANCE_VOTE_EXPIRATION_PERIOD, the votes are removed and the virtual operation:
expired_account_notification_operation is generated.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/12_account_witness_vote.md?ref_type=heads

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/account\_witness\_vote.ts:20

#### Param

**account**

***

### approve

> **approve**: `boolean`

Defined in: wasm/lib/proto/account\_witness\_vote.ts:24

#### Param

**approve**

To vote for the witness, the approve = true. To remove the vote, the approve = false.

***

### witness

> **witness**: `string`

Defined in: wasm/lib/proto/account\_witness\_vote.ts:22

#### Param

**witness**

Witness account.
