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

[src/chain-observers/filters/filter-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/5eab2cad232636d85f195a53901c1212e06f9bee/src/chain-observers/filters/filter-base.ts#L7)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/filters/filter-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/5eab2cad232636d85f195a53901c1212e06f9bee/src/chain-observers/filters/filter-base.ts#L6)
