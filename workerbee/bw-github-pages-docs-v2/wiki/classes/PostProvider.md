[@hiveio/workerbee](../globals) / PostProvider

# Class: PostProvider\<TAccounts\>

## Extends

- `BlogContentProvider`\<`TAccounts`, `IPostProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

## Constructors

### new PostProvider()

> **new PostProvider**\<`TAccounts`\>(): [`PostProvider`](./PostProvider)\<`TAccounts`\>

#### Returns

[`PostProvider`](./PostProvider)\<`TAccounts`\>

#### Overrides

`BlogContentProvider<TAccounts, IPostProviderOptions>.constructor`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:112](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L112)

## Properties

### authors

> `readonly` **authors**: `Map`\<`string`, `undefined` \| `ICommentData`\>

#### Inherited from

`BlogContentProvider.authors`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:42](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L42)

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

#### Inherited from

`BlogContentProvider.isPost`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L43)

## Methods

### createProviderData()

> **createProviderData**(`data`): `Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

#### Inherited from

`BlogContentProvider.createProviderData`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:56](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L56)

***

### provide()

> **provide**(`data`): `Promise`\<[`IPostProviderData`](../interfaces/IPostProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`IPostProviderData`](../interfaces/IPostProviderData)\<`TAccounts`\>\>

#### Overrides

`BlogContentProvider.provide`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:121](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L121)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`IPostProviderOptions`

#### Returns

`void`

#### Overrides

`BlogContentProvider.pushOptions`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:116](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L116)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Inherited from

`BlogContentProvider.usedContexts`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:50](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/chain-observers/providers/blog-content-provider.ts#L50)
