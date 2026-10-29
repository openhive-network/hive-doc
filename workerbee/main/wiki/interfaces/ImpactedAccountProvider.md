[@hiveio/workerbee](../globals) / ImpactedAccountProvider

# Interface: ImpactedAccountProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/impacted-account-provider.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/impacted-account-provider.ts#L21)

## Extends

- `ProviderBase`\<`IImpactedAccountProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

## Properties

### accounts

> `readonly` **accounts**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/impacted-account-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/impacted-account-provider.ts#L22)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IImpactedAccountProviderData`](./IImpactedAccountProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/impacted-account-provider.ts:35](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/impacted-account-provider.ts#L35)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IImpactedAccountProviderData`](./IImpactedAccountProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/impacted-account-provider.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/impacted-account-provider.ts#L24)

#### Parameters

##### options

`IImpactedAccountProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/impacted-account-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/impacted-account-provider.ts#L29)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
