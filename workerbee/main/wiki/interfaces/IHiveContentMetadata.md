[@hiveio/workerbee](../globals) / IHiveContentMetadata

# Interface: IHiveContentMetadata

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:4](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L4)

## Properties

### allowsCurationRewards

> **allowsCurationRewards**: `boolean`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:109](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L109)

Indicates if users who upvote this content are eligible to earn curation rewards.

#### Example

```ts
true
```

***

### allowsReplies

> **allowsReplies**: `boolean`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:97](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L97)

Indicates if other users are allowed to reply to this content.

#### Example

```ts
true
```

***

### allowsVotes

> **allowsVotes**: `boolean`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:103](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L103)

Indicates if other users are allowed to vote on this content.

#### Example

```ts
true
```

***

### author

> **author**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:15](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L15)

The author of the content, usually a Hive account name.

#### Example

```ts
"sagarkothari88"
```

***

### authorRewards

> **authorRewards**: `bigint`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:116](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L116)

The amount of rewards, in Hive Power, that the author received after the payout.
This will be 0 if the post hasn't paid out yet.

#### Example

```ts
0
```

***

### category

> **category**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:9](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L9)

The main topic or community tag for this content.

#### Example

```ts
"hive-106130"
```

***

### curatorPayoutValue

> **curatorPayoutValue**: `asset`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:91](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L91)

The portion of the `totalPayoutValue` that was distributed to "curators" (people who upvoted the content).
This will also show "0" or be empty if the `payoutTime` is in the future.

#### Example

```ts
{ "amount": "0", "nai": "@@000000013", "precision": 3 }
```

***

### isPaid

> **isPaid**: `boolean`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:76](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L76)

Indicates if the content has already paid out rewards.
This will be `true` if the `payoutTime` is in the past, meaning rewards have been distributed.
If the `payoutTime` is in the future, this will be `false`.

#### Example

```ts
true
```

***

### netRshares

> **netRshares**: `bigint`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:52](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L52)

This is a crucial number representing the total "Reward Shares" accumulated by this content from upvotes.
Think of it as the post's "vote weight" or "reward influence." The higher this number,
the greater its potential share of the Hive reward pool. It's not a direct dollar amount
but an internal blockchain measure. The final payout is calculated based on this value
relative to other content paying out at the same time.

#### Example

```ts
150255792948762
```

***

### netVotes

> **netVotes**: `number`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:60](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L60)

The total number of individual upvotes this content has received.
While `netRshares` is more directly tied to rewards (as some votes carry more weight than others),
this shows the raw count of votes.

#### Example

```ts
245
```

***

### parentAuthor

> **parentAuthor**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:34](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L34)

If this content is a reply, this is the author of the content it replies to.
Will be empty if it's a top-level post.

#### Example

```ts
""
```

***

### parentPermlink

> **parentPermlink**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:41](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L41)

If this content is a reply, this is the unique identifier (permlink) of the content it replies to.
Will be the category if it's a reply to the main category feed.

#### Example

```ts
"hive-106130"
```

***

### payoutTime

> **payoutTime**: `Date`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:68](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L68)

The date and time when the rewards for this content are scheduled to be distributed.
This is typically 7 days after the content was created.
Set to "1970-01-01T00:00:00Z" if the content is still pending.

#### Example

```ts
"2025-05-28T23:47:06"
```

***

### permlink

> **permlink**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:21](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L21)

The unique identifier for this content, often called a "permlink."

#### Example

```ts
"mentorship-onboarding-and-how-to-create-an-ezabay-account-for-easily-conversion"
```

***

### title

> **title**: `string`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:27](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L27)

The title of the content. This is usually present for posts, but might be empty for comments.

#### Example

```ts
"Mentorship, onboarding and how to create an Ezabay account for easily conversion."
```

***

### totalPayoutValue

> **totalPayoutValue**: `asset`

Defined in: [src/chain-observers/classifiers/content-metadata-classifier.ts:84](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/classifiers/content-metadata-classifier.ts#L84)

The total value (usually in Hive Backed Dollars - HBD) that was actually paid out for this content.
This will show "0" or be empty if the `payoutTime` is still in the future.
The `amount` is the numerical value, `nai` is the asset identifier, and `precision` is the number of decimal places.

#### Example

```ts
{ "amount": "0", "nai": "@@000000013", "precision": 3 }
```
