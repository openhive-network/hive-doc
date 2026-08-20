[@hiveio/wax](../globals) / transfer

# Interface: transfer

## Brief

Transfers any liquid asset (nonvesting) from one account to another.

Transfer funds from 'from_account' to 'to_account'. HIVE and HBD can be transferred.
Memo for the transaction can be encrypted if message is started with '#'.
Private Memo Key must already be in the wallet for encrypted memo to work.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/02_transfer.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

The amount of asset to transfer from

#### Ref

from_account to

#### Ref

to_account, the allowed currency: HIVE and HBD.

#### Defined in

wasm/lib/proto/transfer.ts:21

***

### from

> **from**: `string`

#### Param

The account the funds are coming from.

#### Defined in

wasm/lib/proto/transfer.ts:17

***

### memo

> **memo**: `string`

#### Param

The memo is plain-text, any encryption on the memo is up to a higher level protocol, must be shorter than 2048.

#### Defined in

wasm/lib/proto/transfer.ts:25

***

### to

> **to**: `string`

#### Param

The account the funds are going to.

#### Defined in

wasm/lib/proto/transfer.ts:19
