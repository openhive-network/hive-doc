[@hiveio/wax](../globals) / escrow\_transfer

# Interface: escrow\_transfer

The escrow allows the account { from_account } to send money to an account { to_account }
only if the agreed terms will be fulfilled. In case of dispute { agent } may divide the funds
between { from } and { to }. The escrow lasts up to { escrow_expiration }.
When the escrow is created, the funds are transferred {from} to a temporary account.
The funds are on the temporary balance, till the operation escrow_release_operation is created.
To create an valid escrow:
1. Sender { from } creates the escrow using the operation: escrow_transfer_operation indicated  { to } and { agent }.
2. The { agent } and { to } have up to { ratification_deadline } for approving the escrow using operation: escrow_approve_operation.
If there is a dispute, the operation: escrow_dispute_operation should be used.
In case of the escrow releases, the operation: escrow_release_operation should be used.

Descritpion https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/27_escrow_transfer.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:26

***

### escrow\_expiration

> **escrow\_expiration**: `string`

#### Param

See description of escrow_release_operation.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:48

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

It is defined by the sender. It should be unique for { from }.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:28

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

The fee amount depends on the agent. The fee is paid to the agent when approved.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:38

***

### from

> **from**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:22

***

### hbd\_amount

> **hbd\_amount**: `undefined` \| [`asset`](./asset)

#### Param

Escrow amount.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:30

***

### hive\_amount

> **hive\_amount**: `undefined` \| [`asset`](./asset)

#### Param

Escrow amount.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:34

***

### json\_meta

> **json\_meta**: `string`

#### Param

json string.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:50

***

### ratification\_deadline

> **ratification\_deadline**: `string`

#### Param

Time for approval for { to } and { agent }.
                                        If the escrow is not approved till { ratification_deadline },
                                        it will be rejected and all funds returned to { from }.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:46

***

### to

> **to**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_transfer.ts:24
