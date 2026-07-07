[@hiveio/wax](../globals) / return\_vesting\_delegation

# Interface: return\_vesting\_delegation

Related to delegate_vesting_shares_operation.
Generated during block processing when process of returning removed or lowered vesting delegation is finished (after return period
passed) and delegator received back his vests.

## Properties

### account

> **account**: `string`

#### Param

delegator (receiver of vesting_shares)

#### Defined in

wasm/lib/proto/return\_vesting\_delegation.ts:13

***

### vesting\_shares

> **vesting\_shares**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) returned delegation

#### Defined in

wasm/lib/proto/return\_vesting\_delegation.ts:15
