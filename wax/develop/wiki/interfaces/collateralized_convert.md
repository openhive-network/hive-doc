[@hiveio/wax](../globals) / collateralized\_convert

# Interface: collateralized\_convert

Defined in: wasm/lib/proto/collateralized\_convert.ts:14

Similar to convert_operation, this operation instructs the blockchain to convert HIVE to HBD.
The operation is performed after 3.5 days, but the owner gets HBD immediately.
The price risk is cushioned by extra HIVE (HIVE_COLLATERAL_RATIO = 200 % ).
After actual conversion takes place the excess HIVE is returned to the owner.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/48_collateralized_convert.md?ref_type=heads

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/collateralized\_convert.ts:20

#### Param

**amount**

Amount > 0, have to be in Hive.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/collateralized\_convert.ts:16

#### Param

**owner**

Account name.

***

### requestid

> **requestid**: `number`

Defined in: wasm/lib/proto/collateralized\_convert.ts:18

#### Param

**requestid**

The number is given by a user. Should be unique for a user.
