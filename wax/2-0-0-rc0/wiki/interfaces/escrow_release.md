[@hiveio/wax](../globals) / escrow\_release

# Interface: escrow\_release

The operation is used to release the funds of the escrow.
The escrow may be released by { from }, { to } or { agent } – depending on the following conditions:
If there is no dispute and escrow has not expired, either party can release funds to the other.
If escrow expires and there is no dispute, either party can release funds to either party.
If there is a dispute regardless of expiration, the agent can release funds to either party
following whichever agreement was in place between the parties.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/29_escrow_release.md?ref_type=heads

## Properties

### agent

> **agent**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_release.ts:22

***

### escrow\_id

> **escrow\_id**: `number`

#### Param

Escrow indicator.

#### Defined in

wasm/lib/proto/escrow\_release.ts:28

***

### from

> **from**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_release.ts:18

***

### hbd\_amount

> **hbd\_amount**: `undefined` \| [`asset`](./asset)

#### Param

The amount of HBD to release.

#### Defined in

wasm/lib/proto/escrow\_release.ts:30

***

### hive\_amount

> **hive\_amount**: `undefined` \| [`asset`](./asset)

#### Param

The amount of HIVE to release.

#### Defined in

wasm/lib/proto/escrow\_release.ts:34

***

### receiver

> **receiver**: `string`

#### Param

The account that should receive funds (might be {from}, might be {to}).

#### Defined in

wasm/lib/proto/escrow\_release.ts:26

***

### to

> **to**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/escrow\_release.ts:20

***

### who

> **who**: `string`

#### Param

The account that is attempting to release the funds.

#### Defined in

wasm/lib/proto/escrow\_release.ts:24
