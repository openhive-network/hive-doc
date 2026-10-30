[@hiveio/workerbee](../globals) / DataEvaluationContext

# Class: DataEvaluationContext

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:17](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L17)

## Constructors

### Constructor

> **new DataEvaluationContext**(`factory`): `DataEvaluationContext`

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L24)

#### Parameters

##### factory

`FactoryBase`

#### Returns

`DataEvaluationContext`

## Methods

### accessStore()

> **accessStore**\<`Classifier`\>(`classifier`): `Classifier`\[`"storeType"`\] *extends* `void` ? `never` : `Classifier`\[`"storeType"`\]

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:92](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L92)

#### Type Parameters

##### Classifier

`Classifier` *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

#### Returns

`Classifier`\[`"storeType"`\] *extends* `void` ? `never` : `Classifier`\[`"storeType"`\]

***

### addTiming()

> **addTiming**(`name`, `time`): `void`

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L28)

#### Parameters

##### name

`string`

##### time

`number`

#### Returns

`void`

***

### get()

> **get**\<`Classifier`\>(`classifier`): `Promise`\<`Classifier`\[`"getType"`\] *extends* `void` ? `never` : `Classifier`\[`"getType"`\]\>

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L43)

#### Type Parameters

##### Classifier

`Classifier` *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

#### Returns

`Promise`\<`Classifier`\[`"getType"`\] *extends* `void` ? `never` : `Classifier`\[`"getType"`\]\>

***

### inject()

> **inject**\<`T`\>(`classifier`, `collector`): `void`

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L32)

#### Type Parameters

##### T

`T` *extends* `IEvaluationContextClass`\<[`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>\>

#### Parameters

##### classifier

`T`

##### collector

`CollectorBase`\<`any`\>

#### Returns

`void`

***

### query()

> **query**\<`Classifier`\>(`classifier`, `collectorOptions`): `Promise`\<`Classifier`\[`"queryType"`\] *extends* `void` ? `never` : `Classifier`\[`"queryType"`\]\>

Defined in: [src/chain-observers/factories/data-evaluation-context.ts:73](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/factories/data-evaluation-context.ts#L73)

#### Type Parameters

##### Classifier

`Classifier` *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

##### collectorOptions

`Classifier`\[`"queryOptionsType"`\]

#### Returns

`Promise`\<`Classifier`\[`"queryType"`\] *extends* `void` ? `never` : `Classifier`\[`"queryType"`\]\>
