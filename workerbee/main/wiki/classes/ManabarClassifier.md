[@hiveio/workerbee](../globals) / ManabarClassifier

# Class: ManabarClassifier

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<`object`, [`IManabarAccountData`](../interfaces/IManabarAccountData), `void`, `void`, `IManabarCollectorOptions`\>

## Constructors

### new ManabarClassifier()

> **new ManabarClassifier**(): [`ManabarClassifier`](./ManabarClassifier)

#### Returns

[`ManabarClassifier`](./ManabarClassifier)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructors)

## Properties

### getType

> **getType**: [`IManabarAccountData`](../interfaces/IManabarAccountData)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

***

### optionsType

> **optionsType**: `IManabarCollectorOptions`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`optionsType`](./CollectorClassifierBase#optionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

***

### queryOptionsType

> **queryOptionsType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryOptionsType`](./CollectorClassifierBase#queryoptionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

***

### queryType

> **queryType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryType`](./CollectorClassifierBase#querytype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

***

### storeType

> **storeType**: `object`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`storeType`](./CollectorClassifierBase#storetype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/collector-classifier-base.ts#L30)

## Methods

### forOptions()

> `static` **forOptions**(`options`): `TRegisterEvaluationContext`

#### Parameters

##### options

`IManabarCollectorOptions`

#### Returns

`TRegisterEvaluationContext`

#### Defined in

[src/chain-observers/classifiers/manabar-classifier.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/classifiers/manabar-classifier.ts#L21)
