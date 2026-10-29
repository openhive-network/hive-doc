[@hiveio/wax](../globals) / decline\_voting\_rights

# Interface: decline\_voting\_rights

Defined in: wasm/lib/proto/decline\_voting\_rights.ts:16

Using the operation decline_voting_rights_operation, a user may decide to decline
their voting rights - for content, witnesses and proposals.
Additionally, a user cannot set a proxy (operation account_witness_proxy_operation).
The operation is done with a HIVE_OWNER_AUTH_RECOVERY_PERIOD day delay.
After HIVE_OWNER_AUTH_RECOVERY_PERIOD days it is irreversible.
During HIVE_OWNER_AUTH_RECOVERY_PERIOD days after creation, the operation may be canceled
using the operation declive_voting_rights_operation with {decline = false}.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/36_decline_voting_rights.md?ref_type=heads

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/decline\_voting\_rights.ts:18

#### Param

**account**

Account name.

***

### decline

> **decline**: `boolean`

Defined in: wasm/lib/proto/decline\_voting\_rights.ts:20

#### Param

**decline**
