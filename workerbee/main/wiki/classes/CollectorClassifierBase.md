[@hiveio/workerbee](../globals) / CollectorClassifierBase

# Class: CollectorClassifierBase\<TStore, TGetResult, TQueryResult, TQueryOptions, TOptions\>

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:14](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L14)

## Extended by

- [`BlockHeaderClassifier`](./BlockHeaderClassifier)
- [`DynamicGlobalPropertiesClassifier`](./DynamicGlobalPropertiesClassifier)
- [`BlockClassifier`](./BlockClassifier)
- [`AccountClassifier`](./AccountClassifier)
- [`RcAccountClassifier`](./RcAccountClassifier)
- [`ImpactedAccountClassifier`](./ImpactedAccountClassifier)
- [`OperationClassifier`](./OperationClassifier)
- [`FeedPriceClassifier`](./FeedPriceClassifier)
- [`WitnessClassifier`](./WitnessClassifier)
- [`ChangeRecoveryInProgressClassifier`](./ChangeRecoveryInProgressClassifier)
- [`DeclineVotingRightsClassifier`](./DeclineVotingRightsClassifier)
- [`ManabarClassifier`](./ManabarClassifier)
- [`ContentMetadataClassifier`](./ContentMetadataClassifier)

## Type Parameters

### TStore

`TStore` *extends* `Record`\<`string`, `any`\> = \{ \}

### TGetResult

`TGetResult` *extends* `void` \| `Record`\<`string`, `any`\> = `void`

### TQueryResult

`TQueryResult` *extends* `void` \| `Record`\<`string`, `any`\> = `void`

### TQueryOptions

`TQueryOptions` *extends* `void` \| `Record`\<`string`, `any`\> = `void`

### TOptions

`TOptions` *extends* `undefined` \| `Record`\<`string`, `any`\> = `undefined`

## Constructors

### Constructor

> **new CollectorClassifierBase**\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>(): `CollectorClassifierBase`\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>

#### Returns

`CollectorClassifierBase`\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>

## Properties

### getType

> **getType**: `TGetResult`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

***

### optionsType

> **optionsType**: `TOptions`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

***

### queryOptionsType

> **queryOptionsType**: `TQueryOptions`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

***

### queryType

> **queryType**: `TQueryResult`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

***

### storeType

> **storeType**: `TStore`

Defined in: [src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/classifiers/collector-classifier-base.ts#L30)
