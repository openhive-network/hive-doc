[@hiveio/workerbee](../globals) / ImpactedAccountProvider

# Class: ImpactedAccountProvider\<TAccounts\>

## Extends

- `ProviderBase`\<`IImpactedAccountProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

## Constructors

### new ImpactedAccountProvider()

> **new ImpactedAccountProvider**\<`TAccounts`\>(): [`ImpactedAccountProvider`](./ImpactedAccountProvider)\<`TAccounts`\>

#### Returns

[`ImpactedAccountProvider`](./ImpactedAccountProvider)\<`TAccounts`\>

#### Inherited from

`ProviderBase<IImpactedAccountProviderOptions>.constructor`

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/impacted-account-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/impacted-account-provider.ts#L22)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IImpactedAccountProviderData`](../interfaces/IImpactedAccountProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IImpactedAccountProviderData`](../interfaces/IImpactedAccountProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/impacted-account-provider.ts:35](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/impacted-account-provider.ts#L35)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`IImpactedAccountProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/impacted-account-provider.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/impacted-account-provider.ts#L24)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/impacted-account-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/impacted-account-provider.ts#L29)
