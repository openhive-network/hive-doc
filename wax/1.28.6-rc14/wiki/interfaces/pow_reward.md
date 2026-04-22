[@hiveio/wax](../globals) / pow\_reward

# Interface: pow\_reward

Related to pow_operation and pow2_operation.
Generated every time one of above operations is executed (up to HF16).
Note: pow2_operation could be executed up to HF17 but mining rewards were stopped after HF16.

## Properties

### reward

> **reward**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS or HIVE) reward for work (HIVE only during first 30 days after genesis)

#### Defined in

wasm/lib/proto/pow\_reward.ts:15

***

### worker

> **worker**: `string`

#### Param

(potentially new) witness that calculated PoW (receiver of reward)

#### Defined in

wasm/lib/proto/pow\_reward.ts:13
