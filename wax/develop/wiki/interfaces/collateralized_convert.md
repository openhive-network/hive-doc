[@hiveio/wax](../globals) / collateralized\_convert

# Interface: collateralized\_convert

Similar to convert_operation, this operation instructs the blockchain to convert HIVE to HBD.
The operation is performed after 3.5 days, but the owner gets HBD immediately.
The price risk is cushioned by extra HIVE (HIVE_COLLATERAL_RATIO = 200 % ).
After actual conversion takes place the excess HIVE is returned to the owner.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/48_collateralized_convert.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

Amount > 0, have to be in Hive.

#### Defined in

wasm/lib/proto/collateralized\_convert.ts:20

***

### owner

> **owner**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/collateralized\_convert.ts:16

***

### requestid

> **requestid**: `number`

#### Param

The number is given by a user. Should be unique for a user.

#### Defined in

wasm/lib/proto/collateralized\_convert.ts:18
