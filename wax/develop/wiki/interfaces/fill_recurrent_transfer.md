[@hiveio/wax](../globals) / fill\_recurrent\_transfer

# Interface: fill\_recurrent\_transfer

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:15

Related to recurrent_transfer_operation.
Generated during block processing starting in the block that included above operation and then after every period
set in the operation until all transfers are executed, too many fail due to shortfall of funds or the transfer is cancelled.
Note: in case of accumulation of very big amount of recurrent transfers to be executed in particular block, some
are going to be postponed to next block(s) and so will be generation of this vop.

## See

failed_recurrent_transfer

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:21

#### Param

**amount**

(HIVE of HBD) amount transferred in current iteration

***

### extensions

> **extensions**: [`recurrent_transfer_extension`](./recurrent_transfer_extension)[]

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:33

#### Param

**extensions**

Extensions. Since HF 28 it may contain the 'pair_id'.
                                                   It allows to define more than one recurrent transfer from sender to the same receiver 'to'.
                                                   Default value 'pair_id=0'.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:17

#### Param

**from\_account**

user that initiated the transfer (source of amount)

***

### memo

> **memo**: `string`

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:25

#### Param

**memo**

memo attached to the transfer

***

### remaining\_executions

> **remaining\_executions**: `number`

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:27

#### Param

**remaining\_executions**

number of remaining pending transferss

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/fill\_recurrent\_transfer.ts:19

#### Param

**to\_account**

user that is target of transfer (receiver of amount)
