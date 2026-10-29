[@hiveio/workerbee](../globals) / CommentProvider

# Interface: CommentProvider\<TAccounts\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:94](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L94)

## Extends

- `BlogContentProvider`\<`TAccounts`, `ICommentProviderOptions`\>

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[] = `TAccountName`[]

## Properties

### authors

> `readonly` **authors**: `Map`\<`string`, `ICommentData` \| `undefined`\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:42](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L42)

#### Inherited from

`BlogContentProvider.authors`

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

Defined in: [src/chain-observers/providers/blog-content-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L43)

#### Inherited from

`BlogContentProvider.isPost`

## Methods

### createProviderData()

> **createProviderData**(`data`): `Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:56](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L56)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`TBlogContentProvided`](../type-aliases/TBlogContentProvided)\<`TAccounts`\>\>

#### Inherited from

`BlogContentProvider.createProviderData`

***

### provide()

> **provide**(`data`): `Promise`\<[`ICommentProviderData`](./ICommentProviderData)\<`TAccounts`\>\>

Defined in: [src/chain-observers/providers/blog-content-provider.ts:104](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L104)

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`ICommentProviderData`](./ICommentProviderData)\<`TAccounts`\>\>

#### Overrides

`BlogContentProvider.provide`

***

### pushOptions()

> **pushOptions**(`options`): `void`

Defined in: [src/chain-observers/providers/blog-content-provider.ts:99](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L99)

#### Parameters

##### options

`ICommentProviderOptions`

#### Returns

`void`

#### Overrides

`BlogContentProvider.pushOptions`

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

Defined in: [src/chain-observers/providers/blog-content-provider.ts:50](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/chain-observers/providers/blog-content-provider.ts#L50)

#### Returns

`TRegisterEvaluationContext`[]

#### Inherited from

`BlogContentProvider.usedContexts`
