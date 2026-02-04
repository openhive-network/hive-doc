[@hiveio/workerbee](../globals) / DataEvaluationContext

# Class: DataEvaluationContext

## Constructors

### new DataEvaluationContext()

> **new DataEvaluationContext**(`factory`): [`DataEvaluationContext`](./DataEvaluationContext)

#### Parameters

##### factory

`FactoryBase`

#### Returns

[`DataEvaluationContext`](./DataEvaluationContext)

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L24)

## Methods

### accessStore()

> **accessStore**\<`Classifier`\>(`classifier`): `Classifier`\[`"storeType"`\] *extends* `void` ? `never` : `Classifier`\[`"storeType"`\]

#### Type Parameters

• **Classifier** *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

#### Returns

`Classifier`\[`"storeType"`\] *extends* `void` ? `never` : `Classifier`\[`"storeType"`\]

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:92](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L92)

***

### addTiming()

> **addTiming**(`name`, `time`): `void`

#### Parameters

##### name

`string`

##### time

`number`

#### Returns

`void`

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L28)

***

### get()

> **get**\<`Classifier`\>(`classifier`): `Promise`\<`Classifier`\[`"getType"`\] *extends* `void` ? `never` : `Classifier`\[`"getType"`\]\>

#### Type Parameters

• **Classifier** *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

#### Returns

`Promise`\<`Classifier`\[`"getType"`\] *extends* `void` ? `never` : `Classifier`\[`"getType"`\]\>

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L43)

***

### inject()

> **inject**\<`T`\>(`classifier`, `collector`): `void`

#### Type Parameters

• **T** *extends* `IEvaluationContextClass`\<[`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>\>

#### Parameters

##### classifier

`T`

##### collector

`CollectorBase`\<`any`\>

#### Returns

`void`

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L32)

***

### query()

> **query**\<`Classifier`\>(`classifier`, `collectorOptions`): `Promise`\<`Classifier`\[`"queryType"`\] *extends* `void` ? `never` : `Classifier`\[`"queryType"`\]\>

#### Type Parameters

• **Classifier** *extends* [`CollectorClassifierBase`](./CollectorClassifierBase)\<`any`, `any`, `any`, `any`, `any`\>

#### Parameters

##### classifier

(...`args`) => `Classifier`

##### collectorOptions

`Classifier`\[`"queryOptionsType"`\]

#### Returns

`Promise`\<`Classifier`\[`"queryType"`\] *extends* `void` ? `never` : `Classifier`\[`"queryType"`\]\>

#### Defined in

[src/chain-observers/factories/data-evaluation-context.ts:73](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/factories/data-evaluation-context.ts#L73)
