[@hiveio/workerbee](../globals) / CommentProvider

# Class: CommentProvider\<TAccounts\>

## Extends

- `BlogContentProvider`\<`TAccounts`, `ICommentProviderOptions`\>

## Type Parameters

• **TAccounts** *extends* `TAccountName`[] = `TAccountName`[]

## Constructors

### new CommentProvider()

> **new CommentProvider**\<`TAccounts`\>(): [`CommentProvider`](./CommentProvider)\<`TAccounts`\>

#### Returns

[`CommentProvider`](./CommentProvider)\<`TAccounts`\>

#### Overrides

`BlogContentProvider<TAccounts, ICommentProviderOptions>.constructor`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:95](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L95)

## Properties

### authors

> `readonly` **authors**: `Map`\<`string`, `undefined` \| `ICommentData`\>

#### Inherited from

`BlogContentProvider.authors`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:42](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L42)

***

### isPost

> `protected` `readonly` **isPost**: `boolean`

#### Inherited from

`BlogContentProvider.isPost`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L43)

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

[src/chain-observers/providers/blog-content-provider.ts:56](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L56)

***

### provide()

> **provide**(`data`): `Promise`\<[`ICommentProviderData`](../interfaces/ICommentProviderData)\<`TAccounts`\>\>

#### Parameters

##### data

`TProviderEvaluationContext`

#### Returns

`Promise`\<[`ICommentProviderData`](../interfaces/ICommentProviderData)\<`TAccounts`\>\>

#### Overrides

`BlogContentProvider.provide`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:104](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L104)

***

### pushOptions()

> **pushOptions**(`options`): `void`

#### Parameters

##### options

`ICommentProviderOptions`

#### Returns

`void`

#### Overrides

`BlogContentProvider.pushOptions`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:99](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L99)

***

### usedContexts()

> **usedContexts**(): `TRegisterEvaluationContext`[]

#### Returns

`TRegisterEvaluationContext`[]

#### Inherited from

`BlogContentProvider.usedContexts`

#### Defined in

[src/chain-observers/providers/blog-content-provider.ts:50](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/chain-observers/providers/blog-content-provider.ts#L50)
