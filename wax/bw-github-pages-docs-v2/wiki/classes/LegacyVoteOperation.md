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

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L12)

## Properties

### voteOperation

> `protected` `readonly` **voteOperation**: [`vote`](../interfaces/vote)

#### Defined in

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L13)

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

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L21)

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

[wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L25)
