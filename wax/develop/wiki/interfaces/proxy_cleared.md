[@hiveio/wax](../globals) / proxy\_cleared

# Interface: proxy\_cleared

Defined in: wasm/lib/proto/proxy\_cleared.ts:23

There are 4 cases( 4 operations ) that can generate `proxy_cleared_operation` virtual operation:

`account_witness_proxy_operation`:
A vop `proxy_cleared_operation` is created in the same block.
We want to set a proxy, but an old proxy exists:
1) {"type":"proxy_cleared_operation","value":{"account":"ACCOUNT","proxy":"OLD-PROXY-ACCOUNT-NAME"}}
We don't want to set a proxy:
2) {"type":"proxy_cleared_operation","value":{"account":"ACCOUNT","proxy":"OLD-PROXY-ACCOUNT-NAME"}}

`decline_voting_rights_operation`:
A vop `proxy_cleared_operation` is generated automatically after `HIVE_OWNER_AUTH_RECOVERY_PERIOD` time ( 30 days ).
3) {"type":"proxy_cleared_operation","value":{"account":"ACCOUNT","proxy":"OLD-PROXY-ACCOUNT-NAME"}}

`update_proposal_votes_operation`, `account_witness_proxy_operation`, `account_witness_vote_operation`:
After HF25 a vop `proxy_cleared_operation` is generated automatically after `HIVE_GOVERNANCE_VOTE_EXPIRATION_PERIOD` time ( 365 days ).
4) {"type":"proxy_cleared_operation","value":{"account":"ACCOUNT","proxy":"OLD-PROXY-ACCOUNT-NAME"}}

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/proxy\_cleared.ts:25

#### Param

**account**

user that sets/unsets a proxy

***

### proxy

> **proxy**: `string`

Defined in: wasm/lib/proto/proxy\_cleared.ts:27

#### Param

**proxy**

proxy user that facilitates voting on witnesses
