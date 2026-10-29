[@hiveio/wax](../globals) / convert

# Interface: convert

Defined in: wasm/lib/proto/convert.ts:12

This operation instructs the blockchain to start a conversion of HBD to Hive.
The funds are deposited after 3.5 days.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/08_convert.md?ref_type=heads

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/convert.ts:18

#### Param

**amount**

Amount > 0, have to be in HBD.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/convert.ts:14

#### Param

**owner**

Account name.

***

### requestid

> **requestid**: `number`

Defined in: wasm/lib/proto/convert.ts:16

#### Param

**requestid**

The number is given by a user. Should be unique for a user.
