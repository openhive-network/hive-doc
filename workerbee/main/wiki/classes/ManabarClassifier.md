[@hiveio/workerbee](../globals) / ManabarClassifier

# Class: ManabarClassifier

Defined in: [src/chain-observers/classifiers/manabar-classifier.ts:20](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/manabar-classifier.ts#L20)

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<\{ \}, [`IManabarAccountData`](../interfaces/IManabarAccountData), `void`, `void`, `IManabarCollectorOptions`\>

## Constructors

### Constructor

> **new ManabarClassifier**(): `ManabarClassifier`

#### Returns

`ManabarClassifier`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructor)

## Properties

### getType

> **getType**: [`IManabarAccountData`](../interfaces/IManabarAccountData)

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

***

### optionsType

> **optionsType**: `IManabarCollectorOptions`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`optionsType`](./CollectorClassifierBase#optionstype)

***

### queryOptionsType

> **queryOptionsType**: `void`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryOptionsType`](./CollectorClassifierBase#queryoptionstype)

***

### queryType

> **queryType**: `void`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryType`](./CollectorClassifierBase#querytype)

***

### storeType

> **storeType**: `object`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L30)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`storeType`](./CollectorClassifierBase#storetype)

## Methods

### forOptions()

> `static` **forOptions**(`options`): `TRegisterEvaluationContext`

Defined in: [src/chain-observers/classifiers/manabar-classifier.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/manabar-classifier.ts#L21)

#### Parameters

##### options

`IManabarCollectorOptions`

#### Returns

`TRegisterEvaluationContext`
