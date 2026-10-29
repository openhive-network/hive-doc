[@hiveio/workerbee](../globals) / ReblogProvider

# Interface: ReblogProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/reblog-provider.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/reblog-provider.ts#L26)

## Extends

- `ProviderBase`\<[`IReblogProviderOptions`](./IReblogProviderOptions)\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `string`[]

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/reblog-provider.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/reblog-provider.ts#L27)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IReblogProviderData`](./IReblogProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/reblog-provider.ts:38](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/reblog-provider.ts#L38)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IReblogProviderData`](./IReblogProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/reblog-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/reblog-provider.ts#L29)

#### Parameters

##### options

[`IReblogProviderOptions`](./IReblogProviderOptions)

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/reblog-provider.ts:34](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/reblog-provider.ts#L34)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
