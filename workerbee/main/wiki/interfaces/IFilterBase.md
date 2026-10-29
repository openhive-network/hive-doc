[@hiveio/workerbee](../globals) / IFilterBase

# Interface: IFilterBase

Defined in: [src/chain-observers/filters/filter-base.ts:5](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/filters/filter-base.ts#L5)

## Methods

### match()

> **match**(`data`): `Promise`\<`boolean`\>

Defined in: [src/chain-observers/filters/filter-base.ts:7](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/filters/filter-base.ts#L7)

#### Parameters

##### data

`TFilterEvaluationContext`

#### Returns

`Promise`\<`boolean`\>

***

### usedContexts()?

> `optional` **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/filters/filter-base.ts:6](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/filters/filter-base.ts#L6)

#### Returns

`TRegisterEvaluationContext`[]
