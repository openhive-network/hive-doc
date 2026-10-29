[@hiveio/wax](../globals) / return\_vesting\_delegation

# Interface: return\_vesting\_delegation

Defined in: wasm/lib/proto/return\_vesting\_delegation.ts:11

Related to delegate_vesting_shares_operation.
Generated during block processing when process of returning removed or lowered vesting delegation is finished (after return period
passed) and delegator received back his vests.

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/return\_vesting\_delegation.ts:13

#### Param

**account**

delegator (receiver of vesting_shares)

***

### vesting\_shares

> **vesting\_shares**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/return\_vesting\_delegation.ts:15

#### Param

**vesting\_shares**

(VESTS) returned delegation
