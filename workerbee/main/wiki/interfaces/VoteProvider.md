[@hiveio/workerbee](../globals) / VoteProvider

# Interface: VoteProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/vote-provider.ts:20](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/vote-provider.ts#L20)

## Extends

- `ProviderBase`\<`IVoteProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

## Properties

### voters

> `readonly` **voters**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/vote-provider.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/vote-provider.ts#L21)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IVoteProviderData`](./IVoteProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/vote-provider.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/vote-provider.ts#L32)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IVoteProviderData`](./IVoteProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/vote-provider.ts:23](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/vote-provider.ts#L23)

#### Parameters

##### options

`IVoteProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/vote-provider.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/vote-provider.ts#L28)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
