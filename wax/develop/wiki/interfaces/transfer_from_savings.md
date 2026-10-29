[@hiveio/wax](../globals) / transfer\_from\_savings

# Interface: transfer\_from\_savings

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:11

Funds withdrawals from the savings to an account take three days.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/33_transfer_from_savings.md?ref_type=heads

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:19

#### Param

**amount**

The allowed currency: HIVE and HBD, amount > 0.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:13

#### Param

**from\_account**

Account name.

***

### memo

> **memo**: `string`

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:23

#### Param

**memo**

Have to be UTF8,  must be shorter than 2048.

***

### request\_id

> **request\_id**: `number`

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:15

#### Param

**request\_id**

The number is given by a user. Should be unique for a user.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/transfer\_from\_savings.ts:17

#### Param

**to\_account**

Account name.
