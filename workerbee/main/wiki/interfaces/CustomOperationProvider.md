[@hiveio/workerbee](../globals) / CustomOperationProvider

# Interface: CustomOperationProvider\<TOperationId\>

Defined in: [src/chain-observers/providers/custom-operation-provider.ts:19](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/custom-operation-provider.ts#L19)

## Extends

- `ProviderBase`\<`ICustomOperationProviderOptions`\>

## Type Parameters

### TOperationId

`TOperationId` *extends* `string`[] = `string`[]

## Properties

### ids

> `readonly` **ids**: `Set`\<`string`\>

Defined in: [src/chain-observers/providers/custom-operation-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/custom-operation-provider.ts#L22)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`ICustomOperationProviderData`](./ICustomOperationProviderData)\<`TOperationId`\>\>

Defined in: [src/chain-observers/providers/custom-operation-provider.ts:33](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/custom-operation-provider.ts#L33)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`ICustomOperationProviderData`](./ICustomOperationProviderData)\<`TOperationId`\>\>

#### Overrides

`ProviderBase.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/custom-operation-provider.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/custom-operation-provider.ts#L24)

#### Parameters

##### options

`ICustomOperationProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/custom-operation-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/custom-operation-provider.ts#L29)

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`
