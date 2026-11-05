[@hiveio/wax](../globals) / OperationBase

# Abstract Class: OperationBase

Defined in: [wasm/lib/detailed/operation\_base.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/operation_base.ts#L8)

## Extended by

- [`HiveAppsOperation`](./HiveAppsOperation)
- [`LegacyVoteOperation`](./LegacyVoteOperation)
- [`UpdateProposalOperation`](./UpdateProposalOperation)
- [`WitnessSetPropertiesOperation`](./WitnessSetPropertiesOperation)
- [`AccountAuthorityUpdateOperation`](./AccountAuthorityUpdateOperation)

## Constructors

### Constructor

> **new OperationBase**(): `OperationBase`

#### Returns

`OperationBase`

## Methods

### finalize()

> `abstract` **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/operation\_base.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/d577f4753a0f64c8d44c7401c48b895fc4c26f93/ts/wasm/lib/detailed/operation_base.ts#L9)

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>
