[@hiveio/wax](../globals) / DefineRecurrentTransferOperation

# Class: DefineRecurrentTransferOperation

## Extends

- `RecurrentTransferOperationBase`

## Constructors

### new DefineRecurrentTransferOperation()

> **new DefineRecurrentTransferOperation**(`data`): [`DefineRecurrentTransferOperation`](./DefineRecurrentTransferOperation)

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

[`DefineRecurrentTransferOperation`](./DefineRecurrentTransferOperation)

#### Overrides

`RecurrentTransferOperationBase.constructor`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:108](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L108)

## Properties

### recurrentTransfer

> `protected` `readonly` **recurrentTransfer**: [`recurrent_transfer`](../interfaces/recurrent_transfer)

#### Inherited from

`RecurrentTransferOperationBase.recurrentTransfer`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L59)

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Inherited from

`RecurrentTransferOperationBase.finalize`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L64)
