[@hiveio/wax](../globals) / recurrent\_transfer

# Interface: recurrent\_transfer

Creates/updates/removes a recurrent transfer in the currency Hive or HBD.
Since HF 28, if user has more than one recurrent transfer to the same receiver
or if user creates the recurrent transfer using pair_id in the extensions,
user has to specify the pair_id in order to update or remove the defined recurrent transfer.
- If amount is set to 0, the recurrent transfer will be deleted and the virtual operation
  fill_recurrent_transfer_operation is not generated
- If there is already a recurrent transfer matching 'from' and 'to', the recurrent transfer will be replaced, but:
- If the 'recurrence' is not changed, the next execution will be according to “old definition”
- If the 'recurrence' is changed, then the next execution will be “update date” + 'recurrence' there is no execution on the update date.
- Up to HF28 there can be only one recurrent transfer for sender 'from' and receiver 'to'.
  Since H28 users may define more recurrent transfers to the same sender and receiver using pair_id in the 'executions'.
- The one account may define up to 255 recurrent transfers to other accounts.
- The execution date of the last transfer should be no more than 730 days in the future.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/49_recurrent_transfer.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

The amount of asset to transfer from

#### Ref

from to

#### Ref

to.
                        If the recurrent transfer failed 10 (HIVE_MAX_CONSECUTIVE_RECURRENT_TRANSFER_FAILURES)
                        times because of the lack of funds, the recurrent transfer will be deleted.
                        Allowed currency: Hive and HBD.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:35

***

### executions

> **executions**: `number`

#### Param

How many times the recurrent payment will be executed.
                             Executions must be at least 2, if you set executions to 1 the recurrent transfer will not be executed.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:50

***

### extensions

> **extensions**: [`recurrent_transfer_extension`](./recurrent_transfer_extension)[]

#### Param

Extensions. Since HF 28 it may contain the 'pair_id'.
                                                   It allows to define more than one recurrent transfer from sender to the same receiver 'to'.
                                                   Default value 'pair_id=0'.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:56

***

### from

> **from**: `string`

#### Param

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:26

***

### memo

> **memo**: `string`

#### Param

must be shorter than 2048.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:39

***

### recurrence

> **recurrence**: `number`

#### Param

How often will the payment be triggered, unit: hours.
                             The first transfer is executed immediately.
                             The minimum value of the parameter is 24 h.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:45

***

### to

> **to**: `string`

#### Param

Account to transfer asset to. Cannot set a transfer to yourself.

#### Defined in

wasm/lib/proto/recurrent\_transfer.ts:28
