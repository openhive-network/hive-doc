[@hiveio/wax](../globals) / RecurrentTransferRemovalOperation

# Class: RecurrentTransferRemovalOperation

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:117](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L117)

## Extends

- `RecurrentTransferOperationBase`

## Constructors

### Constructor

> **new RecurrentTransferRemovalOperation**(`data`): `RecurrentTransferRemovalOperation`

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:135](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L135)

Removes a recurrent transfer in the currency Hive or HBD.
Since HF 28, if user has more than one recurrent transfer to the same receiver
or if user creates the recurrent transfer using pair_id in the extensions,
user has to specify the pair_id in order to remove the defined recurrent transfer.
When invoking this operation, the virtual operation fill_recurrent_transfer_operation is not generated

#### Parameters

##### data

[`IRecurrentTransferRemovalOperationData`](../interfaces/IRecurrentTransferRemovalOperationData)

#### Returns

`RecurrentTransferRemovalOperation`

#### Overrides

`RecurrentTransferOperationBase.constructor`

## Properties

### recurrentTransfer

> `protected` `readonly` **recurrentTransfer**: [`recurrent_transfer`](../interfaces/recurrent_transfer)

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L59)

#### Inherited from

`RecurrentTransferOperationBase.recurrentTransfer`

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/complex\_operations/recurrent\_transfer.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/recurrent_transfer.ts#L121)

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Overrides

`RecurrentTransferOperationBase.finalize`
