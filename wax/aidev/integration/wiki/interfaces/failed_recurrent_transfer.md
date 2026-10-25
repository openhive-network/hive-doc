[@hiveio/wax](../globals) / failed\_recurrent\_transfer

# Interface: failed\_recurrent\_transfer

Related to recurrent_transfer_operation.
Generated during block processing instead of fill_recurrent_transfer_operation when there is not enought funds on from account.
Note: failed transfers are not automatically repeated.
Note: if too many consecutive transfers fail, whole recurrent transfer operation is discontinued.

## See

fill_recurrent_transfer

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE of HBD) amount that was scheduled for transferred in current iteration but failed

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:20

***

### consecutive\_failures

> **consecutive\_failures**: `number`

#### Param

number of failed iterations

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:26

***

### deleted

> **deleted**: `boolean`

#### Param

true if whole recurrent transfer was discontinued due to too many consecutive failures

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:30

***

### extensions

> **extensions**: [`recurrent_transfer_extension`](./recurrent_transfer_extension)[]

#### Param

Extensions. Since HF 28 it may contain the 'pair_id'.
                                                   It allows to define more than one recurrent transfer from sender to the same receiver 'to'.
                                                   Default value 'pair_id=0'.

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:36

***

### from

> **from**: `string`

#### Param

user that initiated the transfer (source of amount that has not enough balance to cover it)

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:16

***

### memo

> **memo**: `string`

#### Param

memo attached to the transfer

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:24

***

### remaining\_executions

> **remaining\_executions**: `number`

#### Param

number of remaining pending transfers

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:28

***

### to

> **to**: `string`

#### Param

user that is target of transfer (would be receiver of amount, but no transfer actually happened)

#### Defined in

wasm/lib/proto/failed\_recurrent\_transfer.ts:18
