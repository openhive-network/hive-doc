[@hiveio/workerbee](../globals) / PostProvider

# Interface: PostProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:111](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L111)

## Extends

- `BlogContentProvider`\<`TAccounts`, `IPostProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

## Properties

### authors

> `readonly` **authors**: `Map`\<`string`, `ICommentData` \| `undefined`\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:42](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L42)

#### Inherited from

`BlogContentProvider.authors`

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

Defined in: [src/chain-observers/providers/blog-content-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L43)

#### Inherited from

`BlogContentProvider.isPost`

## Methods

### createProviderData()

> **createProviderData**(`data`): `Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:56](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L56)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

#### Inherited from

`BlogContentProvider.createProviderData`

***

### provide()

> **provide**(`data`): `Promise`\<[`IPostProviderData`](./IPostProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:121](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L121)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IPostProviderData`](./IPostProviderData)\<`TAccounts`\>\>

#### Overrides

`BlogContentProvider.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/blog-content-provider.ts:116](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L116)

#### Parameters

##### options

`IPostProviderOptions`

#### Returns

`void`

#### Overrides

`BlogContentProvider.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/blog-content-provider.ts:50](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L50)

#### Returns

`TRegisterEvaluationContext`[]

#### Inherited from

`BlogContentProvider.usedContexts`
