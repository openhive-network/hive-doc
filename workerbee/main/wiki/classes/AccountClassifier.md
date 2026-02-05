[@hiveio/workerbee](../globals) / AccountClassifier

# Class: AccountClassifier

## Extends

- [`CollectorClassifierBase`](./CollectorClassifierBase)\<`object`, [`IAccountData`](../interfaces/IAccountData), `void`, `void`, `IAccountCollectorOptions`\>

## Constructors

### new AccountClassifier()

> **new AccountClassifier**(): [`AccountClassifier`](./AccountClassifier)

#### Returns

[`AccountClassifier`](./AccountClassifier)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`constructor`](./CollectorClassifierBase#constructors)

## Properties

### getType

> **getType**: [`IAccountData`](../interfaces/IAccountData)

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`getType`](./CollectorClassifierBase#gettype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

***

### optionsType

> **optionsType**: `IAccountCollectorOptions`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`optionsType`](./CollectorClassifierBase#optionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

***

### queryOptionsType

> **queryOptionsType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryOptionsType`](./CollectorClassifierBase#queryoptionstype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

***

### queryType

> **queryType**: `void`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`queryType`](./CollectorClassifierBase#querytype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

***

### storeType

> **storeType**: `object`

#### Inherited from

[`CollectorClassifierBase`](./CollectorClassifierBase).[`storeType`](./CollectorClassifierBase#storetype)

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/collector-classifier-base.ts#L30)

## Methods

### forOptions()

> `static` **forOptions**(`options`): `TRegisterEvaluationContext`

#### Parameters

##### options

`IAccountCollectorOptions`

#### Returns

`TRegisterEvaluationContext`

#### Defined in

[src/chain-observers/classifiers/account-classifier.ts:55](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/account-classifier.ts#L55)
