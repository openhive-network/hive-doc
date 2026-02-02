[@hiveio/wax](../globals) / IReplyData

# Interface: IReplyData

## Extends

- `Omit`\<[`ICommentData`](./ICommentData), `"jsonMetadata"` \| `"permlink"` \| `"title"`\>

## Properties

### allowCurationRewards?

> `optional` **allowCurationRewards**: `boolean`

Allow or disallow curation rewards for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

#### Inherited from

`Omit.allowCurationRewards`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:100](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L100)

***

### allowVotes?

> `optional` **allowVotes**: `boolean`

Allow or disallow votes for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

#### Inherited from

`Omit.allowVotes`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:107](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L107)

***

### alternativeAuthor?

> `optional` **alternativeAuthor**: `string`

The alternative author of the post.

#### Inherited from

`Omit.alternativeAuthor`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:82](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L82)

***

### author

> **author**: `string`

Account name, the author of the post or the comment.
**It cannot be modified**

#### Inherited from

`Omit.author`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L32)

***

### beneficiaries?

> `optional` **beneficiaries**: [`beneficiary_route_type`](./beneficiary_route_type)[]

The beneficiaries of the post including account and the weight.
Setting this property will create an additional comment_options operation.

#### Inherited from

`Omit.beneficiaries`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:92](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L92)

***

### body

> **body**: `string`

The content of the post or the comment.
**It may be modified**.

#### Inherited from

`Omit.body`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L37)

***

### description?

> `optional` **description**: `string`

The description of the post.

#### Inherited from

`Omit.description`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:70](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L70)

***

### format?

> `optional` **format**: [`ECommentFormat`](../enumerations/ECommentFormat)

The format of the comment.
Currently supported formats are: html, markdown, markdown+html.

#### See

[ECommentFormat](../enumerations/ECommentFormat)

#### Inherited from

`Omit.format`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L66)

***

### images?

> `optional` **images**: `string`[]

The images in the post.

#### Inherited from

`Omit.images`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L78)

***

### jsonMetadata?

> `optional` **jsonMetadata**: `object`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:125](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L125)

***

### links?

> `optional` **links**: `string`[]

The links in the post.

#### Inherited from

`Omit.links`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:74](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L74)

***

### maxAcceptedPayout?

> `optional` **maxAcceptedPayout**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

The maximum accepted payout for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
1_000_000_000
```

#### Inherited from

`Omit.maxAcceptedPayout`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L121)

***

### parentAuthor

> **parentAuthor**: `string`

Account name, the author of the commented post or comment.
If the operation creates a post, it is empty.

#### Inherited from

`Omit.parentAuthor`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L21)

***

### parentPermlink

> **parentPermlink**: `string`

The identifier of the commented post or comment.
When a user creates a post, it may contain the identifier of the community (e.g. hive-174695) or main tag (e.g. travel).
**It cannot be modified**.

#### Inherited from

`Omit.parentPermlink`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L27)

***

### percentHbd?

> `optional` **percentHbd**: `number`

The percentage of the HBD reward.
Setting this property will create an additional comment_options operation.

#### Default

```ts
10000
```

#### Inherited from

`Omit.percentHbd`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:114](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L114)

***

### permlink?

> `optional` **permlink**: `string`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:126](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L126)

***

### tags?

> `optional` **tags**: `string`[]

The tags of the post.

#### Inherited from

`Omit.tags`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L86)

***

### title?

> `optional` **title**: `string`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:127](https://gitlab.syncad.com/hive/wax/-/blob/bd1f12fa00260286397008f44b8c093a8badee63/ts/wasm/lib/detailed/complex_operations/comment.ts#L127)
