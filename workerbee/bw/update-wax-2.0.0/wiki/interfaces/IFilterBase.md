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

[src/chain-observers/filters/filter-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/5a4fea5cf91e40d3722f05ff430c20a9f5a0ca12/src/chain-observers/filters/filter-base.ts#L7)

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Defined in

[src/chain-observers/filters/filter-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/5a4fea5cf91e40d3722f05ff430c20a9f5a0ca12/src/chain-observers/filters/filter-base.ts#L6)
