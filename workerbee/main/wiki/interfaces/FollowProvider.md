[@hiveio/workerbee](../globals) / FollowProvider

# Interface: FollowProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/follow-provider.ts:25](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/follow-provider.ts#L25)

## Extends

- `ProviderBase`\<`IFollowProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `string`[]

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/follow-provider.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/follow-provider.ts#L26)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IFollowProviderData`](./IFollowProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/follow-provider.ts:37](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/follow-provider.ts#L37)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IFollowProviderData`](./IFollowProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/follow-provider.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/follow-provider.ts#L28)

#### Parameters

##### options

`IFollowProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/follow-provider.ts:33](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/follow-provider.ts#L33)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
