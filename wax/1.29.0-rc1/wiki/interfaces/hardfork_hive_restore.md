[@hiveio/wax](../globals) / hardfork\_hive\_restore

# Interface: hardfork\_hive\_restore

Related to hardfork 24.
Generated for every account that was excluded from HF23 airdrop but won appeal.
Note: the late airdrop did not apply properly since HIVE that the accounts should receive did not account for
HIVE from converted VESTS. [how was it resolved?]

## See

hardfork_hive

## Properties

### account

> **account**: `string`

#### Param

account to receive late airdrop (receiver of funds)

#### Defined in

wasm/lib/proto/hardfork\_hive\_restore.ts:15

***

### hbd\_transferred

> **hbd\_transferred**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) part of airdrop (equals related hardfork_hive_operation.hbd_transferred)

#### Defined in

wasm/lib/proto/hardfork\_hive\_restore.ts:19

***

### hive\_transferred

> **hive\_transferred**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) part of airdrop (equals related hardfork_hive_operation.hive_transferred)

#### Defined in

wasm/lib/proto/hardfork\_hive\_restore.ts:23

***

### treasury

> **treasury**: `string`

#### Param

treasury, source of late airdrop

#### Defined in

wasm/lib/proto/hardfork\_hive\_restore.ts:17
