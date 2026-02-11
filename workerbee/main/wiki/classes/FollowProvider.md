[@hiveio/workerbee](../globals) / FollowProvider

# Class: FollowProvider\<TAccounts\>

## Extends

- `ProviderBase`\<`IFollowProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `string`[]

## Constructors

### new FollowProvider()

> **new FollowProvider**\<`TAccounts`\>(): [`FollowProvider`](./FollowProvider)\<`TAccounts`\>

#### Returns

[`FollowProvider`](./FollowProvider)\<`TAccounts`\>

#### Inherited from

`ProviderBase<IFollowProviderOptions>.constructor`

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/follow-provider.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/follow-provider.ts#L26)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IFollowProviderData`](../interfaces/IFollowProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IFollowProviderData`](../interfaces/IFollowProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/follow-provider.ts:37](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/follow-provider.ts#L37)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`IFollowProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/follow-provider.ts:28](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/follow-provider.ts#L28)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/follow-provider.ts:33](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/follow-provider.ts#L33)
