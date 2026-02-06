[@hiveio/workerbee](../globals) / CustomOperationProvider

# Class: CustomOperationProvider\<TOperationId\>

## Extends

- `ProviderBase`\<`ICustomOperationProviderOptions`\>

## Type Parameters

• **TOperationId** *extends* `string`[] = `string`[]

## Constructors

### new CustomOperationProvider()

> **new CustomOperationProvider**\<`TOperationId`\>(): [`CustomOperationProvider`](./CustomOperationProvider)\<`TOperationId`\>

#### Returns

[`CustomOperationProvider`](./CustomOperationProvider)\<`TOperationId`\>

#### Inherited from

`ProviderBase<ICustomOperationProviderOptions>.constructor`

## Properties

### ids

> `readonly` **ids**: `Set`\<`string`\>

#### Defined in

[src/chain-observers/providers/custom-operation-provider.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/custom-operation-provider.ts#L22)

## Methods

### provide()

> **provide**(`data`): `Promise`\<[`ICustomOperationProviderData`](../interfaces/ICustomOperationProviderData)\<`TOperationId`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`ICustomOperationProviderData`](../interfaces/ICustomOperationProviderData)\<`TOperationId`\>\>

#### Overrides

`ProviderBase.provide`

#### Defined in

[src/chain-observers/providers/custom-operation-provider.ts:33](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/custom-operation-provider.ts#L33)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`ICustomOperationProviderOptions`

#### Returns

`void`

#### Overrides

`ProviderBase.pushOptions`

#### Defined in

[src/chain-observers/providers/custom-operation-provider.ts:24](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/custom-operation-provider.ts#L24)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Overrides

`ProviderBase.usedContexts`

#### Defined in

[src/chain-observers/providers/custom-operation-provider.ts:29](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/chain-observers/providers/custom-operation-provider.ts#L29)
