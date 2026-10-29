[@hiveio/wax](../globals) / escrow\_release

# Interface: escrow\_release

Defined in: wasm/lib/proto/escrow\_release.ts:16

The operation is used to release the funds of the escrow.
The escrow may be released by { from }, { to } or { agent } - depending on the following conditions:
If there is no dispute and escrow has not expired, either party can release funds to the other.
If escrow expires and there is no dispute, either party can release funds to either party.
If there is a dispute regardless of expiration, the agent can release funds to either party
following whichever agreement was in place between the parties.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/29_escrow_release.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

Defined in: wasm/lib/proto/escrow\_release.ts:22

#### Param

**agent**

Account name.

***

### escrow\_id

> **escrow\_id**: `number`

Defined in: wasm/lib/proto/escrow\_release.ts:28

#### Param

**escrow\_id**

Escrow indicator.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/escrow\_release.ts:18

#### Param

**from\_account**

Account name.

***

### hbd\_amount

> **hbd\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_release.ts:30

#### Param

**hbd\_amount**

The amount of HBD to release.

***

### hive\_amount

> **hive\_amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/escrow\_release.ts:34

#### Param

**hive\_amount**

The amount of HIVE to release.

***

### receiver

> **receiver**: `string`

Defined in: wasm/lib/proto/escrow\_release.ts:26

#### Param

**receiver**

The account that should receive funds (might be {from}, might be {to}).

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/escrow\_release.ts:20

#### Param

**to\_account**

Account name.

***

### who

> **who**: `string`

Defined in: wasm/lib/proto/escrow\_release.ts:24

#### Param

**who**

The account that is attempting to release the funds.
