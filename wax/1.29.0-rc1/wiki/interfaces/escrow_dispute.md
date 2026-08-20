[@hiveio/wax](../globals) / escrow\_dispute

# Interface: escrow\_dispute

The operation  escrow_dispute_operation is used to raise the dispute. It may be used by { from } or { to } accounts.
If there is a dispute, only {agent} may release the funds.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/28_escrow_dispute.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_dispute.ts:17

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

Escrow identifier.

#### Defined in

wasm/lib/proto/escrow\_dispute.ts:21

***

### from

> **from**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_dispute.ts:13

***

### to

> **to**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_dispute.ts:15

***

### who

> **who**: `string`

#### Param

Account name. Either {to} or {agent}.

#### Defined in

wasm/lib/proto/escrow\_dispute.ts:19
