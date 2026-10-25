[@hiveio/wax](../globals) / fill\_recurrent\_transfer

# Interface: fill\_recurrent\_transfer

Related to recurrent_transfer_operation.
Generated during block processing starting in the block that included above operation and then after every period
set in the operation until all transfers are executed, too many fail due to shortfall of funds or the transfer is cancelled.
Note: in case of accumulation of very big amount of recurrent transfers to be executed in particular block, some
are going to be postponed to next block(s) and so will be generation of this vop.

## See

failed_recurrent_transfer

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE of HBD) amount transferred in current iteration

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:21

***

### extensions

> **extensions**: [`recurrent_transfer_extension`](./recurrent_transfer_extension)[]

#### Param

Extensions. Since HF 28 it may contain the 'pair_id'.
                                                   It allows to define more than one recurrent transfer from sender to the same receiver 'to'.
                                                   Default value 'pair_id=0'.

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:33

***

### from

> **from**: `string`

#### Param

user that initiated the transfer (source of amount)

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:17

***

### memo

> **memo**: `string`

#### Param

memo attached to the transfer

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:25

***

### remaining\_executions

> **remaining\_executions**: `number`

#### Param

number of remaining pending transferss

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:27

***

### to

> **to**: `string`

#### Param

user that is target of transfer (receiver of amount)

#### Defined in

wasm/lib/proto/fill\_recurrent\_transfer.ts:19
