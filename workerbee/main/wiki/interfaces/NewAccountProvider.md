[@hiveio/workerbee](../globals) / NewAccountProvider

# Interface: NewAccountProvider

Defined in: [src/chain-observers/providers/new-account-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/new-account-provider.ts#L22)

## Extends

- `ProviderBase`

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`INewAccountProviderData`](./INewAccountProviderData)\>

Defined in: [src/chain-observers/providers/new-account-provider.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/new-account-provider.ts#L27)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`INewAccountProviderData`](./INewAccountProviderData)\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()?

> `optional` **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/provider-base.ts:15](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L15)

#### Parameters

##### options

\{ \}

#### Returns

`void`

#### Inherited from

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/new-account-provider.ts:23](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/new-account-provider.ts#L23)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
