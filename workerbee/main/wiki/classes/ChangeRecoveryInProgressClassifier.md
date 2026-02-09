[@hiveio/workerbee](../globals) / ChangeRecoveryInProgressClassifier

# Class: ChangeRecoveryInProgressClassifier

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<`object`, `IChangeRecoveryInProgressData`, `void`, `void`, `IChangeRecoveryCollectorOptions`\>

## Constructors

### new ChangeRecoveryInProgressClassifier()

> **new ChangeRecoveryInProgressClassifier**(): [`ChangeRecoveryInProgressClassifier`](./ChangeRecoveryInProgressClassifier)

#### Returns

[`ChangeRecoveryInProgressClassifier`](./ChangeRecoveryInProgressClassifier)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructors)

## Properties

### getType

> **getType**: `IChangeRecoveryInProgressData`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

***

### optionsType

> **optionsType**: `IChangeRecoveryCollectorOptions`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`optionsType`](./CollectorClassifierBase#optionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

***

### queryOptionsType

> **queryOptionsType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryOptionsType`](./CollectorClassifierBase#queryoptionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

***

### queryType

> **queryType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryType`](./CollectorClassifierBase#querytype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

***

### storeType

> **storeType**: `object`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`storeType`](./CollectorClassifierBase#storetype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/collector-classifier-base.ts#L30)

## Methods

### forOptions()

> `static` **forOptions**(`options`): `TRegisterEvaluationContext`

#### Parameters

##### options

`IChangeRecoveryCollectorOptions`

#### Returns

`TRegisterEvaluationContext`

#### Defined in

[src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/classifiers/change-recovery-in-progress-classifier.ts#L24)
