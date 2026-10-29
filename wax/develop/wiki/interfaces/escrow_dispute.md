[@hiveio/wax](../globals) / escrow\_dispute

# Interface: escrow\_dispute

Defined in: wasm/lib/proto/escrow\_dispute.ts:11

The operation  escrow_dispute_operation is used to raise the dispute. It may be used by { from } or { to } accounts.
If there is a dispute, only {agent} may release the funds.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/28_escrow_dispute.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

Defined in: wasm/lib/proto/escrow\_dispute.ts:17

#### Param

**agent**

Account name.

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_dispute.ts:21

#### Param

**escrow\_id**

Escrow identifier.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_dispute.ts:13

#### Param

**from\_account**

Account name.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_dispute.ts:15

#### Param

**to\_account**

Account name.

***

### who

> **who**: `string`

Defined in: wasm/lib/proto/escrow\_dispute.ts:19

#### Param

**who**

Account name. Either {to} or {agent}.
