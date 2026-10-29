[@hiveio/wax](../globals) / escrow\_rejected

# Interface: escrow\_rejected

Defined in: wasm/lib/proto/escrow\_rejected.ts:13

Related to escrow_approve_operation and escrow_transfer_operation.
Generated when pending escrow transfer is cancelled and user that initiated it receives all the funds back.
It can happen with explicit rejection with use of first operation. Can also happen during block processing when either
agent or to account failed to approve before ratification deadline.

## See

escrow_approved

## Properties

### agent

> **agent**: `string`

Defined in: wasm/lib/proto/escrow\_rejected.ts:19

#### Param

**agent**

user that was designated as agent of cancelled escrow transfer

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_rejected.ts:21

#### Param

**escrow\_id**

id of cancelled escrow transfer

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_rejected.ts:31

#### Param

**fee**

(HIVE of HBD) fee from cancelled escrow transfer (same amount as in escrow_transfer_operation)

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_rejected.ts:15

#### Param

**from\_account**

user that initiated escrow transfer (receiver of all the funds)

***

### hbd\_amount

> **hbd\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_rejected.ts:23

#### Param

**hbd\_amount**

(HBD) funds from cancelled escrow transfer (same amount as in escrow_transfer_operation)

***

### hive\_amount

> **hive\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_rejected.ts:27

#### Param

**hive\_amount**

(HIVE) funds from cancelled escrow transfer (same amount as in escrow_transfer_operation)

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_rejected.ts:17

#### Param

**to\_account**

user that was target of cancelled escrow transfer
