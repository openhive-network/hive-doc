[@hiveio/workerbee](../globals) / ReblogProvider

# Class: ReblogProvider\<TAccounts\>

## Extends

- `ProviderBase`\<[`IReblogProviderOptions`](../interfaces/IReblogProviderOptions)\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `string`[]

## Constructors

### new ReblogProvider()

> **new ReblogProvider**\<`TAccounts`\>(): [`ReblogProvider`](./ReblogProvider)\<`TAccounts`\>

#### Returns

[`ReblogProvider`](./ReblogProvider)\<`TAccounts`\>

#### Inherited from

`ProviderBase<IReblogProviderOptions>.constructor`

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/reblog-provider.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/chain-observers/providers/reblog-provider.ts#L27)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IReblogProviderData`](../interfaces/IReblogProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IReblogProviderData`](../interfaces/IReblogProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/reblog-provider.ts:38](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/chain-observers/providers/reblog-provider.ts#L38)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

[`IReblogProviderOptions`](../interfaces/IReblogProviderOptions)

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/reblog-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/chain-observers/providers/reblog-provider.ts#L29)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/reblog-provider.ts:34](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/chain-observers/providers/reblog-provider.ts#L34)
