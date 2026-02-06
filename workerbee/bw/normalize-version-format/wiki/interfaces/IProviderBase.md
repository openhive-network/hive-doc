[@hiveio/workerbee](../globals) / IProviderBase

# Interface: IProviderBase\<IOptions\>

## Type Parameters

• **IOptions** *extends* `object` = \{\}

## Methods

### provide()

> **provide**(`data`): `Promise`\<`object`\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`object`\>

#### Defined in

[src/chain-observers/providers/provider-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/provider-base.ts#L7)

***

### pushOptions()?

> `optional` **pushOptions**(`options`): `void`

#### Parameters

##### options

`IOptions`

#### Returns

`void`

#### Defined in

[src/chain-observers/providers/provider-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/provider-base.ts#L6)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/providers/provider-base.ts:5](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/provider-base.ts#L5)
