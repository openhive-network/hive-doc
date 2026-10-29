[@hiveio/wax](../globals) / failed\_recurrent\_transfer

# Interface: failed\_recurrent\_transfer

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:14

Related to recurrent_transfer_operation.
Generated during block processing instead of fill_recurrent_transfer_operation when there is not enought funds on from account.
Note: failed transfers are not automatically repeated.
Note: if too many consecutive transfers fail, whole recurrent transfer operation is discontinued.

## See

fill_recurrent_transfer

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:20

#### Param

**amount**

(HIVE of HBD) amount that was scheduled for transferred in current iteration but failed

***

### consecutive\_failures

> **consecutive\_failures**: `number`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:26

#### Param

**consecutive\_failures**

number of failed iterations

***

### deleted

> **deleted**: `boolean`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:30

#### Param

**deleted**

true if whole recurrent transfer was discontinued due to too many consecutive failures

***

### extensions

> **extensions**: [`recurrent_transfer_extension`](./recurrent_transfer_extension)[]

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:36

#### Param

**extensions**

Extensions. Since HF 28 it may contain the 'pair_id'.
                                                   It allows to define more than one recurrent transfer from sender to the same receiver 'to'.
                                                   Default value 'pair_id=0'.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:16

#### Param

**from\_account**

user that initiated the transfer (source of amount that has not enough balance to cover it)

***

### memo

> **memo**: `string`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:24

#### Param

**memo**

memo attached to the transfer

***

### remaining\_executions

> **remaining\_executions**: `number`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:28

#### Param

**remaining\_executions**

number of remaining pending transfers

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/failed\_recurrent\_transfer.ts:18

#### Param

**to\_account**

user that is target of transfer (would be receiver of amount, but no transfer actually happened)
