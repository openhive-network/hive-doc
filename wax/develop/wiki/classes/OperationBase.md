[@hiveio/wax](../globals) / OperationBase

# Class: `abstract` OperationBase

## Extended by

- [`HiveAppsOperation`](./HiveAppsOperation)
- [`LegacyVoteOperation`](./LegacyVoteOperation)
- [`UpdateProposalOperation`](./UpdateProposalOperation)
- [`WitnessSetPropertiesOperation`](./WitnessSetPropertiesOperation)
- [`AccountAuthorityUpdateOperation`](./AccountAuthorityUpdateOperation)

## Constructors

### new OperationBase()

> **new OperationBase**(): [`OperationBase`](./OperationBase)

#### Returns

[`OperationBase`](./OperationBase)

## Methods

### finalize()

> `abstract` **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Defined in

[wasm/lib/detailed/operation\_base.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/be3d61a927ecf9f69336abe55b17b3e3903e1d75/ts/wasm/lib/detailed/operation_base.ts#L9)
