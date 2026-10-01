[@hiveio/wax](../globals) / escrow\_rejected

# Interface: escrow\_rejected

Related to escrow_approve_operation and escrow_transfer_operation.
Generated when pending escrow transfer is cancelled and user that initiated it receives all the funds back.
It can happen with explicit rejection with use of first operation. Can also happen during block processing when either
agent or to account failed to approve before ratification deadline.

## See

escrow_approved

## Properties

### agent

> **agent**: `string`

#### Param

user that was designated as agent of cancelled escrow transfer

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:19

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

id of cancelled escrow transfer

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:21

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE of HBD) fee from cancelled escrow transfer (same amount as in escrow_transfer_operation)

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:31

***

### from

> **from**: `string`

#### Param

user that initiated escrow transfer (receiver of all the funds)

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:15

***

### hbd\_amount

> **hbd\_amount**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) funds from cancelled escrow transfer (same amount as in escrow_transfer_operation)

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:23

***

### hive\_amount

> **hive\_amount**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) funds from cancelled escrow transfer (same amount as in escrow_transfer_operation)

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:27

***

### to

> **to**: `string`

#### Param

user that was target of cancelled escrow transfer

#### Defined in

wasm/lib/proto/escrow\_rejected.ts:17
