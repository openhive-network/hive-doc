[@hiveio/wax](../globals) / transfer\_to\_vesting\_completed

# Interface: transfer\_to\_vesting\_completed

Related to transfer_to_vesting_operation.
Generated every time above operation is executed. Supplements it with amount of VESTS received.
Note: power up immediately increases mana regeneration and vote power for comments, but there is a grace period before
it activates as governance vote power.

## See

delayed_voting

## Properties

### from\_account

> **from\_account**: `string`

#### Param

account that executed power up (source of hive_vested)

#### Defined in

wasm/lib/proto/transfer\_to\_vesting\_completed.ts:15

***

### hive\_vested

> **hive\_vested**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) liquid funds being turned into VESTS

#### Defined in

wasm/lib/proto/transfer\_to\_vesting\_completed.ts:19

***

### to\_account

> **to\_account**: `string`

#### Param

account that gets power up (receiver of vesting_shares_received)

#### Defined in

wasm/lib/proto/transfer\_to\_vesting\_completed.ts:17

***

### vesting\_shares\_received

> **vesting\_shares\_received**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) result of power up

#### Defined in

wasm/lib/proto/transfer\_to\_vesting\_completed.ts:23
