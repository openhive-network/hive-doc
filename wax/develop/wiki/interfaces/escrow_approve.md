[@hiveio/wax](../globals) / escrow\_approve

# Interface: escrow\_approve

Defined in: wasm/lib/proto/escrow\_approve.ts:15

The operation escrow_approve_operation is used to approve the escrow.
The approval should be done by { to } and by the { agent }.
The escrow approval is irreversible.
If { agent } or { to } haven't approved the escrow before the { ratification_deadline} or either
of them explicitly rejected the escrow, the escrow is rejected.
If {agent} and {to} have approved the escrow, the {fee} is transferred from temporary balance to {agent} account.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/31_escrow_approve.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

Defined in: wasm/lib/proto/escrow\_approve.ts:21

#### Param

**agent**

Account name.

***

### approve

> **approve**: `boolean`

Defined in: wasm/lib/proto/escrow\_approve.ts:27

#### Param

**approve**

approve = true; (approve = false explicitly rejects the escrow)

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_approve.ts:25

#### Param

**escrow\_id**

Escrow identifier.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_approve.ts:17

#### Param

**from\_account**

Account name.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_approve.ts:19

#### Param

**to\_account**

Account name.

***

### who

> **who**: `string`

Defined in: wasm/lib/proto/escrow\_approve.ts:23

#### Param

**who**

Account name. Either {to} or {agent}.
