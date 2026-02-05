[@hiveio/workerbee](../globals) / VoteProvider

# Class: VoteProvider\<TAccounts\>

## Extends

- `ProviderBase`\<`IVoteProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

## Constructors

### new VoteProvider()

> **new VoteProvider**\<`TAccounts`\>(): [`VoteProvider`](./VoteProvider)\<`TAccounts`\>

#### Returns

[`VoteProvider`](./VoteProvider)\<`TAccounts`\>

#### Inherited from

`ProviderBase<IVoteProviderOptions>.constructor`

## Properties

### voters

> `readonly` **voters**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/vote-provider.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/providers/vote-provider.ts#L21)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IVoteProviderData`](../interfaces/IVoteProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IVoteProviderData`](../interfaces/IVoteProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/vote-provider.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/providers/vote-provider.ts#L32)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`IVoteProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/vote-provider.ts:23](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/providers/vote-provider.ts#L23)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/vote-provider.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/providers/vote-provider.ts#L28)
