[@hiveio/wax](../globals) / transfer\_from\_savings

# Interface: transfer\_from\_savings

Funds withdrawals from the savings to an account take three days.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/33_transfer_from_savings.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

The allowed currency: HIVE and HBD, amount > 0.

#### Defined in

wasm/lib/proto/transfer\_from\_savings.ts:19

***

### from

> **from**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/transfer\_from\_savings.ts:13

***

### memo

> **memo**: `string`

#### Param

Have to be UTF8,  must be shorter than 2048.

#### Defined in

wasm/lib/proto/transfer\_from\_savings.ts:23

***

### request\_id

> **request\_id**: `number`

#### Param

The number is given by a user. Should be unique for a user.

#### Defined in

wasm/lib/proto/transfer\_from\_savings.ts:15

***

### to

> **to**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/transfer\_from\_savings.ts:17
