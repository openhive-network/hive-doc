[@hiveio/wax](../globals) / hardfork\_hive\_restore

# Interface: hardfork\_hive\_restore

Defined in: wasm/lib/proto/hardfork\_hive\_restore.ts:13

Related to hardfork 24.
Generated for every account that was excluded from HF23 airdrop but won appeal.
Note: the late airdrop did not apply properly since HIVE that the accounts should receive did not account for
HIVE from converted VESTS. [how was it resolved?]

## See

hardfork_hive

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/hardfork\_hive\_restore.ts:15

#### Param

**account**

account to receive late airdrop (receiver of funds)

***

### hbd\_transferred

> **hbd\_transferred**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive\_restore.ts:19

#### Param

**hbd\_transferred**

(HBD) part of airdrop (equals related hardfork_hive_operation.hbd_transferred)

***

### hive\_transferred

> **hive\_transferred**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive\_restore.ts:23

#### Param

**hive\_transferred**

(HIVE) part of airdrop (equals related hardfork_hive_operation.hive_transferred)

***

### treasury

> **treasury**: `string`

Defined in: wasm/lib/proto/hardfork\_hive\_restore.ts:17

#### Param

**treasury**

treasury, source of late airdrop
