[@hiveio/workerbee](../globals) / AccountClassifier

# Class: AccountClassifier

Defined in: [src/chain-observers/classifiers/account-classifier.ts:54](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/account-classifier.ts#L54)

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<\{ \}, [`IAccountData`](../interfaces/IAccountData), `void`, `void`, `IAccountCollectorOptions`\>

## Constructors

### Constructor

> **new AccountClassifier**(): `AccountClassifier`

#### Returns

`AccountClassifier`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructor)

## Properties

### getType

> **getType**: [`IAccountData`](../interfaces/IAccountData)

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

***

### optionsType

> **optionsType**: `IAccountCollectorOptions`

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

Defined in: [src/chain-observers/classifiers/account-classifier.ts:55](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/account-classifier.ts#L55)

#### Parameters

##### options

`IAccountCollectorOptions`

#### Returns

`TRegisterEvaluationContext`
