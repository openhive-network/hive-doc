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

[src/chain-observers/filters/filter-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/filters/filter-base.ts#L7)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/filters/filter-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/filters/filter-base.ts#L6)
