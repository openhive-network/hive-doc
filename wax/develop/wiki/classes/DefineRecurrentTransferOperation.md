[@hiveio/wax](../globals) / DefineRecurrentTransferOperation

# Class: DefineRecurrentTransferOperation

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:91](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L91)

## Extends

- `RecurrentTransferOperationBase`

## Constructors

### Constructor

> **new DefineRecurrentTransferOperation**(`data`): `DefineRecurrentTransferOperation`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:108](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L108)

Creates/updates a recurrent transfer in the currency Hive or HBD.
 * Since HF 28, if user has more than one recurrent transfer to the same receiver
 * or if user creates the recurrent transfer using pairId in the extensions,
 * user has to specify the pairId in order to update the defined recurrent transfer.
 *
 * Amount cannot be 0 when defining / updating recurrent transfer.
 *
 * If there is already a recurrent transfer matching 'from' and 'to', the recurrent transfer will be replaced, but:
 * - If the 'recurrence' is not changed, the next execution will be according to “old definition”
 * - If the 'recurrence' is changed, then the next execution will be “update date” + 'recurrence' there is no execution on the update date.
 * - Up to HF28 there can be only one recurrent transfer for sender 'from' and receiver 'to'.
 *   Since H28 users may define more recurrent transfers to the same sender and receiver using pair_id in the 'executions'.
 * - The one account may define up to 255 recurrent transfers to other accounts.
 * - The execution date of the last transfer should be no more than 730 days in the future.

#### Parameters

##### data

[`IRecurrentTransferData`](../interfaces/IRecurrentTransferData)

#### Returns

`DefineRecurrentTransferOperation`

#### Overrides

`RecurrentTransferOperationBase.constructor`

## Properties

### recurrentTransfer

> `protected` `readonly` **recurrentTransfer**: [`recurrent_transfer`](../interfaces/recurrent_transfer)

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L59)

#### Inherited from

`RecurrentTransferOperationBase.recurrentTransfer`

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L64)

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Inherited from

`RecurrentTransferOperationBase.finalize`
