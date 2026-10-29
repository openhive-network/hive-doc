[@hiveio/wax](../globals) / transfer\_to\_vesting\_completed

# Interface: transfer\_to\_vesting\_completed

Defined in: wasm/lib/proto/transfer\_to\_vesting\_completed.ts:13

Related to transfer_to_vesting_operation.
Generated every time above operation is executed. Supplements it with amount of VESTS received.
Note: power up immediately increases mana regeneration and vote power for comments, but there is a grace period before
it activates as governance vote power.

## See

delayed_voting

## Properties

### from\_account

> **from\_account**: `string`

Defined in: wasm/lib/proto/transfer\_to\_vesting\_completed.ts:15

#### Param

**from\_account**

account that executed power up (source of hive_vested)

***

### hive\_vested

> **hive\_vested**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/transfer\_to\_vesting\_completed.ts:19

#### Param

**hive\_vested**

(HIVE) liquid funds being turned into VESTS

***

### to\_account

> **to\_account**: `string`

Defined in: wasm/lib/proto/transfer\_to\_vesting\_completed.ts:17

#### Param

**to\_account**

account that gets power up (receiver of vesting_shares_received)

***

### vesting\_shares\_received

> **vesting\_shares\_received**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/transfer\_to\_vesting\_completed.ts:23

#### Param

**vesting\_shares\_received**

(VESTS) result of power up
