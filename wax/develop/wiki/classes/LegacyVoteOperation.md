[@hiveio/wax](../globals) / LegacyVoteOperation

# Class: LegacyVoteOperation

Defined in: [wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L11)

## Extends

- [`OperationBase`](./OperationBase)

## Constructors

### Constructor

> **new LegacyVoteOperation**(`voteOperation`): `LegacyVoteOperation`

Defined in: [wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L12)

#### Parameters

##### voteOperation

[`vote`](../interfaces/vote)

#### Returns

`LegacyVoteOperation`

#### Overrides

[`OperationBase`](./OperationBase).[`constructor`](./OperationBase#constructor)

## Properties

### voteOperation

> `protected` `readonly` **voteOperation**: [`vote`](../interfaces/vote)

Defined in: [wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L13)

## Methods

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L21)

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Overrides

[`OperationBase`](./OperationBase).[`finalize`](./OperationBase#finalize)

***

### for()

> `static` **for**(`chain`, `voter`, `author`, `permlink`, `weightPercent?`): `Promise`\<`LegacyVoteOperation`\>

Defined in: [wasm/lib/detailed/complex\_operations/legacy\_vote\_operation.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/complex_operations/legacy_vote_operation.ts#L25)

#### Parameters

##### chain

[`IHiveChainInterface`](../interfaces/IHiveChainInterface)

##### voter

`string`

##### author

`string`

##### permlink

`string`

##### weightPercent?

`number` = `100`

#### Returns

`Promise`\<`LegacyVoteOperation`\>
