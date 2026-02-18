[@hiveio/wax](../globals) / BlogPostOperation

# Class: BlogPostOperation

Same as the comment base, but requires user to set the category (parent permlink) on the comment

## Extends

- `CommentOperation`

## Constructors

### new BlogPostOperation()

> **new BlogPostOperation**(`data`): [`BlogPostOperation`](./BlogPostOperation)

#### Parameters

##### data

[`IArticle`](../interfaces/IArticle)

#### Returns

[`BlogPostOperation`](./BlogPostOperation)

#### Overrides

`CommentOperation.constructor`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:337](https://gitlab.syncad.com/hive/wax/-/blob/f73f483d5c38a28ebc5e72b9fcff623d1cf9e30d/ts/wasm/lib/detailed/complex_operations/comment.ts#L337)

## Properties

### comment

> `protected` `readonly` **comment**: [`comment`](../interfaces/comment)

#### Inherited from

`CommentOperation.comment`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:137](https://gitlab.syncad.com/hive/wax/-/blob/f73f483d5c38a28ebc5e72b9fcff623d1cf9e30d/ts/wasm/lib/detailed/complex_operations/comment.ts#L137)

***

### jsonMetadata

> `protected` **jsonMetadata**: `Record`\<`string`, `any`\>

#### Inherited from

`CommentOperation.jsonMetadata`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:140](https://gitlab.syncad.com/hive/wax/-/blob/f73f483d5c38a28ebc5e72b9fcff623d1cf9e30d/ts/wasm/lib/detailed/complex_operations/comment.ts#L140)

## Methods

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Inherited from

`CommentOperation.finalize`

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/f73f483d5c38a28ebc5e72b9fcff623d1cf9e30d/ts/wasm/lib/detailed/complex_operations/comment.ts#L149)

***

### pushMetadataProperty()

> **pushMetadataProperty**(`keyOrObject`, `value`?): `this`

Assigns given object or sets given value on key in comment meta values

#### Parameters

##### keyOrObject

key to set the value on or the entire object of key-value pairs to assign to the json metadata object

`string` | `object`

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

#### Defined in

[wasm/lib/detailed/complex\_operations/comment.ts:267](https://gitlab.syncad.com/hive/wax/-/blob/f73f483d5c38a28ebc5e72b9fcff623d1cf9e30d/ts/wasm/lib/detailed/complex_operations/comment.ts#L267)
