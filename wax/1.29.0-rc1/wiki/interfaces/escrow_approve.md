[@hiveio/wax](../globals) / escrow\_approve

# Interface: escrow\_approve

The operation escrow_approve_operation is used to approve the escrow.
The approval should be done by { to } and by the { agent }.
The escrow approval is irreversible.
If { agent } or { to } haven’t approved the escrow before the { ratification_deadline} or either
of them explicitly rejected the escrow, the escrow is rejected.
If {agent} and {to} have approved the escrow, the {fee} is transferred from temporary balance to {agent} account.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/31_escrow_approve.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_approve.ts:21

***

### approve

> **approve**: `boolean`

#### Param

approve = true; (approve = false explicitly rejects the escrow)

#### Defined in

wasm/lib/proto/escrow\_approve.ts:27

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

Escrow identifier.

#### Defined in

wasm/lib/proto/escrow\_approve.ts:25

***

### from

> **from**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_approve.ts:17

***

### to

> **to**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_approve.ts:19

***

### who

> **who**: `string`

#### Param

Account name. Either {to} or {agent}.

#### Defined in

wasm/lib/proto/escrow\_approve.ts:23
