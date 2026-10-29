[@hiveio/wax](../globals) / liquidity\_reward

# Interface: liquidity\_reward

Defined in: wasm/lib/proto/liquidity\_reward.ts:12

Related to limit_order_create_operation and limit_order_create2_operation.
Generated during block processing to indicate reward paid to the market makers on internal HIVE<->HBD market.
No longer active after HF12.

## See

fill_order_operation

## Properties

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/liquidity\_reward.ts:14

#### Param

**owner**

market maker (receiver of payout)

***

### payout

> **payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/liquidity\_reward.ts:16

#### Param

**payout**

(HIVE) reward for provided liquidity
