[@hiveio/wax](../globals) / escrow\_approved

# Interface: escrow\_approved

Defined in: wasm/lib/proto/escrow\_approved.ts:11

Related to escrow_approve_operation.
Generated when both agent and to accounts approved pending escrow transfer (agent receives fee).

## See

escrow_rejected

## Properties

### agent

> **agent**: `string`

Defined in: wasm/lib/proto/escrow\_approved.ts:17

#### Param

**agent**

user that is an agent of pending escrow transfer (receiver of fee)

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_approved.ts:19

#### Param

**escrow\_id**

id of escrow transfer

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_approved.ts:21

#### Param

**fee**

(HIVE of HBD) fee paid to agent

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_approved.ts:13

#### Param

**from\_account**

user that initiated escrow transfer

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_approved.ts:15

#### Param

**to\_account**

user that is target of pending escrow transfer
