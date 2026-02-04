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

[src/chain-observers/providers/impacted-account-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/impacted-account-provider.ts#L22)

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

[src/chain-observers/providers/impacted-account-provider.ts:35](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/impacted-account-provider.ts#L35)

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

[src/chain-observers/providers/impacted-account-provider.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/impacted-account-provider.ts#L24)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/impacted-account-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/ef496d9c96e74fe07bdfc5743dc58495a42eee68/src/chain-observers/providers/impacted-account-provider.ts#L29)
