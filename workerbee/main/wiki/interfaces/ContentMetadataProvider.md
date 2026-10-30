[@hiveio/workerbee](../globals) / ContentMetadataProvider

# Abstract Interface: ContentMetadataProvider\<TAccounts, TOptions\>

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:31](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L31)

## Extends

- `ProviderBase`\<`TOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

### TOptions

`TOptions` *extends* `object` = `object`

## Properties

### authors

> `readonly` **authors**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:35](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L35)

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:36](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L36)

## Methods

### createProviderData()

> **createProviderData**(`data`): `Promise`\<`Partial`\<[`TContentMetadataProvided`](../type-aliases/TContentMetadataProvided)\<`TAccounts`\>\>\>

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:49](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L49)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`Partial`\<[`TContentMetadataProvided`](../type-aliases/TContentMetadataProvided)\<`TAccounts`\>\>\>

***

### provide()

> `abstract` **provide**(`data`): `Promise`\<`object`\>

Defined in: [src/chain-observers/providers/provider-base.ts:17](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/provider-base.ts#L17)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`object`\>

#### Inherited from

`ProviderBase.provide`

***

### pushOptions()

> `abstract` **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:47](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L47)

#### Parameters

##### options

`TOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/content-metadata-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/content-metadata-provider.ts#L43)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
