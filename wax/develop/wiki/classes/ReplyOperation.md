[@hiveio/wax](../globals) / ReplyOperation

# Class: ReplyOperation

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:316](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L316)

Same as the comment base, but requires parentAuthor and parentPermlink to be set

## Extends

- `CommentOperation`

## Constructors

### Constructor

> **new ReplyOperation**(`data`): `ReplyOperation`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:317](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L317)

#### Parameters

##### data

[`IReplyData`](../interfaces/IReplyData)

#### Returns

`ReplyOperation`

#### Overrides

`CommentOperation.constructor`

## Properties

### comment

> `protected` `readonly` **comment**: [`comment`](../interfaces/comment)

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:137](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L137)

#### Inherited from

`CommentOperation.comment`

***

### jsonMetadata

> `protected` **jsonMetadata**: `Record`\<`string`, `any`\>

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:140](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L140)

#### Inherited from

`CommentOperation.jsonMetadata`

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L149)

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Inherited from

`CommentOperation.finalize`

***

### pushMetadataProperty()

> **pushMetadataProperty**(`keyOrObject`, `value?`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/comment.ts:267](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/comment.ts#L267)

Assigns given object or sets given value on key in comment meta values

#### Parameters

##### keyOrObject

`string` \| `object`

key to set the value on or the entire object of key-value pairs to assign to the json metadata object

##### value?

`any`

value to be set (optional when passing the entire object)

#### Returns

`this`

itself

#### Throws

if key already exists on the jsonmetadata object

#### Inherited from

`CommentOperation.pushMetadataProperty`
