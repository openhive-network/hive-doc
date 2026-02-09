[@hiveio/workerbee](../globals) / ManabarProvider

# Class: ManabarProvider\<TAccounts\>

## Extends

- `ProviderBase`\<`IManabarProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

## Constructors

### new ManabarProvider()

> **new ManabarProvider**\<`TAccounts`\>(): [`ManabarProvider`](./ManabarProvider)\<`TAccounts`\>

#### Returns

[`ManabarProvider`](./ManabarProvider)\<`TAccounts`\>

#### Inherited from

`ProviderBase<IManabarProviderOptions>.constructor`

## Properties

### manabarData

> `readonly` **manabarData**: `Map`\<`string`, `Set`\<`EManabarType`\>\>

#### Defined in

[src/chain-observers/providers/manabar-provider.ts:20](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/providers/manabar-provider.ts#L20)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IManabarProviderData`](../interfaces/IManabarProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IManabarProviderData`](../interfaces/IManabarProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/manabar-provider.ts:41](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/providers/manabar-provider.ts#L41)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`IManabarProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/manabar-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/providers/manabar-provider.ts#L22)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/manabar-provider.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/3dea0e6c6cad7461308332944c53e8f69fe2f812/src/chain-observers/providers/manabar-provider.ts#L32)
