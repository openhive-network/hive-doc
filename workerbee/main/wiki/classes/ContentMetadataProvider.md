[@hiveio/workerbee](../globals) / ContentMetadataProvider

# Class: `abstract` ContentMetadataProvider\<TAccounts, TOptions\>

## Extends

- `ProviderBase`\<`TOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

• **TOptions** *extends* `object` = `object`

## Constructors

### new ContentMetadataProvider()

> **new ContentMetadataProvider**\<`TAccounts`, `TOptions`\>(`isPost`): [`ContentMetadataProvider`](./ContentMetadataProvider)\<`TAccounts`, `TOptions`\>

#### Parameters

##### isPost

`boolean`

#### Returns

[`ContentMetadataProvider`](./ContentMetadataProvider)\<`TAccounts`, `TOptions`\>

#### Overrides

`ProviderBase<TOptions>.constructor`

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:38](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L38)

## Properties

### authors

> `readonly` **authors**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:35](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L35)

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:36](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L36)

## Methods

### createProviderData()

> **createProviderData**(`data`): `Promise`\<`Partial`\<[`TContentMetadataProvided`](../type-aliases/TContentMetadataProvided)\<`TAccounts`\>\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`Partial`\<[`TContentMetadataProvided`](../type-aliases/TContentMetadataProvided)\<`TAccounts`\>\>\>

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:49](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L49)

***

### provide()

> `abstract` **provide**(`data`): `Promise`\<`object`\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<`object`\>

#### Inherited from

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/provider-base.ts:17](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/provider-base.ts#L17)

***

### pushOptions()

> `abstract` **pushOptions**(`options`): `void`

#### Parameters

##### options

`TOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:47](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L47)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/content-metadata-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/d6dcf4229bbf793dd6bd36e74404691b693d4a39/src/chain-observers/providers/content-metadata-provider.ts#L43)
