[@hiveio/wax](../globals) / RecurrentTransferRemovalOperation

# Class: RecurrentTransferRemovalOperation

## Extends

- `RecurrentTransferOperationBase`

## Constructors

### new RecurrentTransferRemovalOperation()

> **new RecurrentTransferRemovalOperation**(`data`): [`RecurrentTransferRemovalOperation`](./RecurrentTransferRemovalOperation)

Removes a recurrent transfer in the currency Hive or HBD.
Since HF 28, if user has more than one recurrent transfer to the same receiver
or if user creates the recurrent transfer using pair_id in the extensions,
user has to specify the pair_id in order to remove the defined recurrent transfer.
When invoking this operation, the virtual operation fill_recurrent_transfer_operation is not generated

#### Parameters

##### data

[`IRecurrentTransferRemovalOperationData`](../interfaces/IRecurrentTransferRemovalOperationData)

#### Returns

[`RecurrentTransferRemovalOperation`](./RecurrentTransferRemovalOperation)

#### Overrides

`RecurrentTransferOperationBase.constructor`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:135](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L135)

## Properties

### recurrentTransfer

> `protected` `readonly` **recurrentTransfer**: [`recurrent_transfer`](../interfaces/recurrent_transfer)

#### Inherited from

`RecurrentTransferOperationBase.recurrentTransfer`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L59)

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Overrides

`RecurrentTransferOperationBase.finalize`

#### Defined in

[wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L121)
