[@hiveio/workerbee](../globals) / CollectorClassifierBase

# Class: CollectorClassifierBase\<TStore, TGetResult, TQueryResult, TQueryOptions, TOptions\>

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

• **TStore** *extends* `Record`\<`string`, `any`\> = \{\}

• **TGetResult** *extends* `void` \| `Record`\<`string`, `any`\> = `void`

• **TQueryResult** *extends* `void` \| `Record`\<`string`, `any`\> = `void`

• **TQueryOptions** *extends* `void` \| `Record`\<`string`, `any`\> = `void`

• **TOptions** *extends* `undefined` \| `Record`\<`string`, `any`\> = `undefined`

## Constructors

### new CollectorClassifierBase()

> **new CollectorClassifierBase**\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>(): [`CollectorClassifierBase`](./CollectorClassifierBase)\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>

#### Returns

[`CollectorClassifierBase`](./CollectorClassifierBase)\<`TStore`, `TGetResult`, `TQueryResult`, `TQueryOptions`, `TOptions`\>

## Properties

### getType

> **getType**: `TGetResult`

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/classifiers/collector-classifier-base.ts#L26)

***

### optionsType

> **optionsType**: `TOptions`

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/classifiers/collector-classifier-base.ts#L29)

***

### queryOptionsType

> **queryOptionsType**: `TQueryOptions`

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/classifiers/collector-classifier-base.ts#L28)

***

### queryType

> **queryType**: `TQueryResult`

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/classifiers/collector-classifier-base.ts#L27)

***

### storeType

> **storeType**: `TStore`

#### Defined in

[src/chain-observers/classifiers/collector-classifier-base.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/classifiers/collector-classifier-base.ts#L30)
