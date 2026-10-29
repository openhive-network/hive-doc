[@hiveio/wax](../globals) / escrow\_transfer

# Interface: escrow\_transfer

Defined in: wasm/lib/proto/escrow\_transfer.ts:20

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

Defined in: wasm/lib/proto/escrow\_transfer.ts:26

#### Param

**agent**

Account name.

***

### escrow\_expiration

> **escrow\_expiration**: `string`

Defined in: wasm/lib/proto/escrow\_transfer.ts:48

#### Param

**escrow\_expiration**

See description of escrow_release_operation.

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_transfer.ts:28

#### Param

**escrow\_id**

It is defined by the sender. It should be unique for { from }.

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_transfer.ts:38

#### Param

**fee**

The fee amount depends on the agent. The fee is paid to the agent when approved.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_transfer.ts:22

#### Param

**from\_account**

Account name.

***

### hbd\_amount

> **hbd\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_transfer.ts:30

#### Param

**hbd\_amount**

Escrow amount.

***

### hive\_amount

> **hive\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_transfer.ts:34

#### Param

**hive\_amount**

Escrow amount.

***

### json\_meta

> **json\_meta**: `string`

Defined in: wasm/lib/proto/escrow\_transfer.ts:50

#### Param

**json\_meta**

json string.

***

### ratification\_deadline

> **ratification\_deadline**: `string`

Defined in: wasm/lib/proto/escrow\_transfer.ts:46

#### Param

**ratification\_deadline**

Time for approval for { to } and { agent }.
                                        If the escrow is not approved till { ratification_deadline },
                                        it will be rejected and all funds returned to { from }.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_transfer.ts:24

#### Param

**to\_account**

Account name.
