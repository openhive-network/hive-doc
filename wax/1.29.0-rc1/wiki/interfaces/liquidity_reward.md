[@hiveio/wax](../globals) / liquidity\_reward

# Interface: liquidity\_reward

Related to limit_order_create_operation and limit_order_create2_operation.
Generated during block processing to indicate reward paid to the market makers on internal HIVE<->HBD market.
No longer active after HF12.

## See

fill_order_operation

## Properties

### owner

> **owner**: `string`

#### Param

market maker (receiver of payout)

#### Defined in

wasm/lib/proto/liquidity\_reward.ts:14

***

### payout

> **payout**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) reward for provided liquidity

#### Defined in

wasm/lib/proto/liquidity\_reward.ts:16
