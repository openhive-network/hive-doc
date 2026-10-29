[@hiveio/workerbee](../globals) / ChangeRecoveryInProgressClassifier

# Class: ChangeRecoveryInProgressClassifier

Defined in: [src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts:17](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts#L17)

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<\{ \}, `IChangeRecoveryInProgressData`, `void`, `void`, `IChangeRecoveryCollectorOptions`\>

## Constructors

### Constructor

> **new ChangeRecoveryInProgressClassifier**(): `ChangeRecoveryInProgressClassifier`

#### Returns

`ChangeRecoveryInProgressClassifier`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructor)

## Properties

### getType

> **getType**: `IChangeRecoveryInProgressData`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

***

### optionsType

> **optionsType**: `IChangeRecoveryCollectorOptions`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`optionsType`](./CollectorClassifierBase#optionstype)

***

### queryOptionsType

> **queryOptionsType**: `void`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryOptionsType`](./CollectorClassifierBase#queryoptionstype)

***

### queryType

> **queryType**: `void`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryType`](./CollectorClassifierBase#querytype)

***

### storeType

> **storeType**: `object`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/collector-classifier-base.ts#L30)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`storeType`](./CollectorClassifierBase#storetype)

## Methods

### forOptions()

> `static` **forOptions**(`options`): `TRegisterEvaluationContext`

Defined in: [src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts#L24)

#### Parameters

##### options

`IChangeRecoveryCollectorOptions`

#### Returns

`TRegisterEvaluationContext`
