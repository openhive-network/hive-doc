[@hiveio/workerbee](../globals) / ManabarProvider

# Interface: ManabarProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/manabar-provider.ts:19](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/manabar-provider.ts#L19)

## Extends

- `ProviderBase`\<`IManabarProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

## Properties

### manabarData

> `readonly` **manabarData**: `Map`\<`string`, `Set`\<`EManabarType`\>\>

Defined in: [src/chain-observers/providers/manabar-provider.ts:20](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/manabar-provider.ts#L20)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`IManabarProviderData`](./IManabarProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/manabar-provider.ts:41](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/manabar-provider.ts#L41)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IManabarProviderData`](./IManabarProviderData)\<`TAccounts`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/manabar-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/manabar-provider.ts#L22)

#### Parameters

##### options

`IManabarProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/manabar-provider.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/manabar-provider.ts#L32)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
