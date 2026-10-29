[@hiveio/wax](../globals) / IReplyData

# Interface: IReplyData

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:124](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L124)

## Extends

- `Omit`\<[`ICommentData`](./ICommentData), `"jsonMetadata"` \| `"permlink"` \| `"title"`\>

## Properties

### allowCurationRewards?

> `optional` **allowCurationRewards?**: `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:100](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L100)

Allow or disallow curation rewards for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

#### Inherited from

[`ICommentData`](./ICommentData).[`allowCurationRewards`](./ICommentData#allowcurationrewards)

***

### allowVotes?

> `optional` **allowVotes?**: `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:107](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L107)

Allow or disallow votes for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

#### Inherited from

[`ICommentData`](./ICommentData).[`allowVotes`](./ICommentData#allowvotes)

***

### alternativeAuthor?

> `optional` **alternativeAuthor?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:82](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L82)

The alternative author of the post.

#### Inherited from

[`ICommentData`](./ICommentData).[`alternativeAuthor`](./ICommentData#alternativeauthor)

***

### author

> **author**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L32)

Account name, the author of the post or the comment.
**It cannot be modified**

#### Inherited from

[`ICommentData`](./ICommentData).[`author`](./ICommentData#author)

***

### beneficiaries?

> `optional` **beneficiaries?**: [`beneficiary_route_type`](./beneficiary_route_type)[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:92](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L92)

The beneficiaries of the post including account and the weight.
Setting this property will create an additional comment_options operation.

#### Inherited from

[`ICommentData`](./ICommentData).[`beneficiaries`](./ICommentData#beneficiaries)

***

### body

> **body**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L37)

The content of the post or the comment.
**It may be modified**.

#### Inherited from

[`ICommentData`](./ICommentData).[`body`](./ICommentData#body)

***

### description?

> `optional` **description?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:70](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L70)

The description of the post.

#### Inherited from

[`ICommentData`](./ICommentData).[`description`](./ICommentData#description)

***

### format?

> `optional` **format?**: [`ECommentFormat`](../enumerations/ECommentFormat)

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L66)

The format of the comment.
Currently supported formats are: html, markdown, markdown+html.

#### See

[ECommentFormat](../enumerations/ECommentFormat)

#### Inherited from

[`ICommentData`](./ICommentData).[`format`](./ICommentData#format)

***

### images?

> `optional` **images?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L78)

The images in the post.

#### Inherited from

[`ICommentData`](./ICommentData).[`images`](./ICommentData#images)

***

### jsonMetadata?

> `optional` **jsonMetadata?**: `object`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:125](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L125)

***

### links?

> `optional` **links?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:74](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L74)

The links in the post.

#### Inherited from

[`ICommentData`](./ICommentData).[`links`](./ICommentData#links)

***

### maxAcceptedPayout?

> `optional` **maxAcceptedPayout?**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L121)

The maximum accepted payout for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
1_000_000_000
```

#### Inherited from

[`ICommentData`](./ICommentData).[`maxAcceptedPayout`](./ICommentData#maxacceptedpayout)

***

### parentAuthor

> **parentAuthor**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L21)

Account name, the author of the commented post or comment.
If the operation creates a post, it is empty.

#### Inherited from

[`ICommentData`](./ICommentData).[`parentAuthor`](./ICommentData#parentauthor)

***

### parentPermlink

> **parentPermlink**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L27)

The identifier of the commented post or comment.
When a user creates a post, it may contain the identifier of the community (e.g. hive-174695) or main tag (e.g. travel).
**It cannot be modified**.

#### Inherited from

[`ICommentData`](./ICommentData).[`parentPermlink`](./ICommentData#parentpermlink)

***

### percentHbd?

> `optional` **percentHbd?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:114](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L114)

The percentage of the HBD reward.
Setting this property will create an additional comment_options operation.

#### Default

```ts
10000
```

#### Inherited from

[`ICommentData`](./ICommentData).[`percentHbd`](./ICommentData#percenthbd)

***

### permlink?

> `optional` **permlink?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:126](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L126)

***

### tags?

> `optional` **tags?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L86)

The tags of the post.

#### Inherited from

[`ICommentData`](./ICommentData).[`tags`](./ICommentData#tags)

***

### title?

> `optional` **title?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:127](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/comment.ts#L127)
