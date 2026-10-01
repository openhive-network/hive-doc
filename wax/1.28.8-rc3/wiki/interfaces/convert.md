[@hiveio/wax](../globals) / convert

# Interface: convert

This operation instructs the blockchain to start a conversion of HBD to Hive.
The funds are deposited after 3.5 days.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/08_convert.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

Amount > 0, have to be in HBD.

#### Defined in

wasm/lib/proto/convert.ts:18

***

### owner

> **owner**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/convert.ts:14

***

### requestid

> **requestid**: `number`

#### Param

The number is given by a user. Should be unique for a user.

#### Defined in

wasm/lib/proto/convert.ts:16
