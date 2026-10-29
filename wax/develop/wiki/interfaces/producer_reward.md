[@hiveio/wax](../globals) / producer\_reward

# Interface: producer\_reward

Defined in: wasm/lib/proto/producer\_reward.ts:10

Related to block processing.
Generated during block processing every block for current witness.

## Properties

### producer

> **producer**: `string`

Defined in: wasm/lib/proto/producer\_reward.ts:12

#### Param

**producer**

witness (receiver of vesting_shares)

***

### vesting\_shares

> **vesting\_shares**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/producer\_reward.ts:14

#### Param

**vesting\_shares**

(VESTS or HIVE) reward for block production (HIVE only during first 30 days after genesis)
