[@hiveio/workerbee](../globals) / NewAccountProvider

# Class: NewAccountProvider

## Extends

- `ProviderBase`

## Constructors

### new NewAccountProvider()

> **new NewAccountProvider**(): [`NewAccountProvider`](./NewAccountProvider)

#### Returns

[`NewAccountProvider`](./NewAccountProvider)

#### Inherited from

`ProviderBase.constructor`

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`INewAccountProviderData`](../interfaces/INewAccountProviderData)\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`INewAccountProviderData`](../interfaces/INewAccountProviderData)\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/new-account-provider.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/7102bee5a92d018a9d6b843a050bb6ddedc77d63/src/chain-observers/providers/new-account-provider.ts#L27)

***

### pushOptions()?

> `optional` **pushOptions**(`options`): `void`

#### Parameters

##### options

#### Returns

`void`

#### Inherited from

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/provider-base.ts:15](https://gitlab.syncad.com/hive/workerbee/-/blob/7102bee5a92d018a9d6b843a050bb6ddedc77d63/src/chain-observers/providers/provider-base.ts#L15)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/new-account-provider.ts:23](https://gitlab.syncad.com/hive/workerbee/-/blob/7102bee5a92d018a9d6b843a050bb6ddedc77d63/src/chain-observers/providers/new-account-provider.ts#L23)
