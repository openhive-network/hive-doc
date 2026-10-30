[@hiveio/workerbee](../globals) / IProviderBase

# Interface: IProviderBase\<IOptions\>

Defined in: [src/chain-observers/providers/provider-base.ts:4](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L4)

## Type Parameters

### IOptions

`IOptions` *extends* `object` = \{ \}

## Methods

### provide()

> **provide**(`data`): `Promise`\<`object`\>

Defined in: [src/chain-observers/providers/provider-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L7)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`object`\>

***

### pushOptions()?

> `optional` **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/provider-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L6)

#### Parameters

##### options

`IOptions`

#### Returns

`void`

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/provider-base.ts:5](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L5)

#### Returns

`TRegisterEvaluationContext`[]
