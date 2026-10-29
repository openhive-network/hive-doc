[@hiveio/wax](../globals) / ICommentData

# Interface: ICommentData

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L16)

## Properties

### allowCurationRewards?

> `optional` **allowCurationRewards?**: `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:100](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L100)

Allow or disallow curation rewards for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

***

### allowVotes?

> `optional` **allowVotes?**: `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:107](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L107)

Allow or disallow votes for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
true
```

***

### alternativeAuthor?

> `optional` **alternativeAuthor?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:82](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L82)

The alternative author of the post.

***

### author

> **author**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L32)

Account name, the author of the post or the comment.
**It cannot be modified**

***

### beneficiaries?

> `optional` **beneficiaries?**: [`beneficiary_route_type`](./beneficiary_route_type)[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:92](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L92)

The beneficiaries of the post including account and the weight.
Setting this property will create an additional comment_options operation.

***

### body

> **body**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L37)

The content of the post or the comment.
**It may be modified**.

***

### description?

> `optional` **description?**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:70](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L70)

The description of the post.

***

### format?

> `optional` **format?**: [`ECommentFormat`](../enumerations/ECommentFormat)

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L66)

The format of the comment.
Currently supported formats are: html, markdown, markdown+html.

#### See

[ECommentFormat](../enumerations/ECommentFormat)

***

### images?

> `optional` **images?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L78)

The images in the post.

***

### jsonMetadata

> **jsonMetadata**: `object`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:48](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L48)

There is no blockchain validation on json_metadata, but the structure has been established by the community.
From the blockchain point of view it is a json file.
For the second layer, the following keys may be used:
- app, e.g. peakd/2023.2.3
- format, e.g. markdown
- tags, e.g. photography
- users
- images

***

### links?

> `optional` **links?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:74](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L74)

The links in the post.

***

### maxAcceptedPayout?

> `optional` **maxAcceptedPayout?**: [`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L121)

The maximum accepted payout for the post.
Setting this property will create an additional comment_options operation.

#### Default

```ts
1_000_000_000
```

***

### parentAuthor

> **parentAuthor**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:21](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L21)

Account name, the author of the commented post or comment.
If the operation creates a post, it is empty.

***

### parentPermlink

> **parentPermlink**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L27)

The identifier of the commented post or comment.
When a user creates a post, it may contain the identifier of the community (e.g. hive-174695) or main tag (e.g. travel).
**It cannot be modified**.

***

### percentHbd?

> `optional` **percentHbd?**: `number`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:114](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L114)

The percentage of the HBD reward.
Setting this property will create an additional comment_options operation.

#### Default

```ts
10000
```

***

### permlink

> **permlink**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L53)

Unique to the author, the identifier of the post or comment.
**It cannot be modified**.

***

### tags?

> `optional` **tags?**: `string`[]

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L86)

The tags of the post.

***

### title

> **title**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:58](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L58)

The title of the submitted post, in case of the comment, is often empty.
**It may be modified**.
