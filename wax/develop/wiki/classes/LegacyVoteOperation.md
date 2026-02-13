[@hiveio/wax](../globals) / LegacyVoteOperation

# Class: LegacyVoteOperation

## Extends

- [`OperationBase`](./OperationBase)

## Constructors

### new LegacyVoteOperation()

> **new LegacyVoteOperation**(`voteOperation`): [`LegacyVoteOperation`](./LegacyVoteOperation)

#### Parameters

##### voteOperation

[`vote`](../interfaces/vote)

#### Returns

[`LegacyVoteOperation`](./LegacyVoteOperation)

#### Overrides

[`OperationBase`](./OperationBase).[`constructor`](./OperationBase#constructors)

#### Defined in

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/bf3eec1cb090d565a6022f7f980f6259bba7b2ac/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L12)

## Properties

### voteOperation

> `protected` `readonly` **voteOperation**: [`vote`](../interfaces/vote)

#### Defined in

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/bf3eec1cb090d565a6022f7f980f6259bba7b2ac/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L13)

## Methods

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Overrides

[`OperationBase`](./OperationBase).[`finalize`](./OperationBase#finalize)

#### Defined in

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/bf3eec1cb090d565a6022f7f980f6259bba7b2ac/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L21)

***

### for()

> `static` **for**(`chain`, `voter`, `author`, `permlink`, `weightPercent`): `Promise`\<[`LegacyVoteOperation`](./LegacyVoteOperation)\>

#### Parameters

##### chain

[`IHiveChainInterface`](../interfaces/IHiveChainInterface)

##### voter

`string`

##### author

`string`

##### permlink

`string`

##### weightPercent

`number` = `100`

#### Returns

`Promise`\<[`LegacyVoteOperation`](./LegacyVoteOperation)\>

#### Defined in

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/bf3eec1cb090d565a6022f7f980f6259bba7b2ac/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L25)
