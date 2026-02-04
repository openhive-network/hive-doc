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

[src/chain-observers/providers/provider-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/provider-base.ts#L7)

***

### pushOptions()?

> `optional` **pushOptions**(`options`): `void`

#### Parameters

##### options

`IOptions`

#### Returns

`void`

#### Defined in

[src/chain-observers/providers/provider-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/provider-base.ts#L6)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/providers/provider-base.ts:5](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/provider-base.ts#L5)
