[@hiveio/workerbee](../globals) / IFilterBase

# Interface: IFilterBase

## Methods

### match()

> **match**(`data`): `Promise`\<`boolean`\>

#### Parameters

##### data

`TFilterEvaluationContext`

#### Returns

`Promise`\<`boolean`\>

#### Defined in

[src/chain-observers/filters/filter-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/fb60e1d5c2be40756d833b36480b9d3eabe9b5bc/src/chain-observers/filters/filter-base.ts#L7)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/filters/filter-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/fb60e1d5c2be40756d833b36480b9d3eabe9b5bc/src/chain-observers/filters/filter-base.ts#L6)
