[@hiveio/wax](../globals) / producer\_reward

# Interface: producer\_reward

Related to block processing.
Generated during block processing every block for current witness.

## Properties

### producer

> **producer**: `string`

#### Param

witness (receiver of vesting_shares)

#### Defined in

wasm/lib/proto/producer\_reward.ts:12

***

### vesting\_shares

> **vesting\_shares**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS or HIVE) reward for block production (HIVE only during first 30 days after genesis)

#### Defined in

wasm/lib/proto/producer\_reward.ts:14
