[@hiveio/wax](../globals) / dhf\_conversion

# Interface: dhf\_conversion

Defined in: wasm/lib/proto/dhf\_conversion.ts:12

Related to specific case of transfer_operation and to block processing.
When user transferred HIVE to treasury the amount is immediately converted to HBD and this vops is generated.
Also generated during block processing every day during daily proposal maintenance.
Note: portion of HIVE on treasury balance is converted to HBD and thus increases funds available for proposals.

## Properties

### hbd\_amount\_out

> **hbd\_amount\_out**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/dhf\_conversion.ts:20

#### Param

**hbd\_amount\_out**

(HBD) effect of conversion

***

### hive\_amount\_in

> **hive\_amount\_in**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/dhf\_conversion.ts:16

#### Param

**hive\_amount\_in**

(HIVE) source of conversion

***

### treasury

> **treasury**: `string`

Defined in: wasm/lib/proto/dhf\_conversion.ts:14

#### Param

**treasury**

treasury (source of hive_amount_in and receiver of hbd_amount_out)
