[@hiveio/wax](../globals) / dhf\_conversion

# Interface: dhf\_conversion

Related to specific case of transfer_operation and to block processing.
When user transferred HIVE to treasury the amount is immediately converted to HBD and this vops is generated.
Also generated during block processing every day during daily proposal maintenance.
Note: portion of HIVE on treasury balance is converted to HBD and thus increases funds available for proposals.

## Properties

### hbd\_amount\_out

> **hbd\_amount\_out**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) effect of conversion

#### Defined in

wasm/lib/proto/dhf\_conversion.ts:20

***

### hive\_amount\_in

> **hive\_amount\_in**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) source of conversion

#### Defined in

wasm/lib/proto/dhf\_conversion.ts:16

***

### treasury

> **treasury**: `string`

#### Param

treasury (source of hive_amount_in and receiver of hbd_amount_out)

#### Defined in

wasm/lib/proto/dhf\_conversion.ts:14
