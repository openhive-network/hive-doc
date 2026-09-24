[@hiveio/wax](../globals) / escrow\_approved

# Interface: escrow\_approved

Related to escrow_approve_operation.
Generated when both agent and to accounts approved pending escrow transfer (agent receives fee).

## See

escrow_rejected

## Properties

### agent

> **agent**: `string`

#### Param

user that is an agent of pending escrow transfer (receiver of fee)

#### Defined in

wasm/lib/proto/escrow\_approved.ts:17

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

id of escrow transfer

#### Defined in

wasm/lib/proto/escrow\_approved.ts:19

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE of HBD) fee paid to agent

#### Defined in

wasm/lib/proto/escrow\_approved.ts:21

***

### from

> **from**: `string`

#### Param

user that initiated escrow transfer

#### Defined in

wasm/lib/proto/escrow\_approved.ts:13

***

### to

> **to**: `string`

#### Param

user that is target of pending escrow transfer

#### Defined in

wasm/lib/proto/escrow\_approved.ts:15
