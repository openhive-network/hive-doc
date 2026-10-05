[@hiveio/wax](../globals) / comment

# Interface: comment

Using comment operation a user may create a post or a comment.
From the blockchain point of view, it is the same operation – always comment.
If a comment has no parent, it is a post.
The parent of the comment may be a post or a comment.
Users may comment their own comments.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/01_comment.md?ref_type=heads

## Properties

### author

> **author**: `string`

#### Param

Account name, the author of the post or the comment.
                         It cannot be modified.

#### Defined in

wasm/lib/proto/comment.ts:32

***

### body

> **body**: `string`

#### Param

The content of the post or the comment.
                       It may be modified.

#### Defined in

wasm/lib/proto/comment.ts:47

***

### json\_metadata

> **json\_metadata**: `string`

#### Param

There is no blockchain validation on json_metadata,
                                but the structure has been established by the community.
                                From the blockchain point of view it is a json file.
                                For the second layer, the following keys may be used:
                                - app, e.g. peakd/2023.2.3
                                - format, e.g. markdown
                                - tags, e.g. photography
                                - users
                                - images

#### Defined in

wasm/lib/proto/comment.ts:59

***

### parent\_author

> **parent\_author**: `string`

#### Param

Account name, the author of the commented post or comment.
                                If the operation creates a post, it is empty.
                                It cannot be modified.

#### Defined in

wasm/lib/proto/comment.ts:20

***

### parent\_permlink

> **parent\_permlink**: `string`

#### Param

The identifier of the commented post or comment.
                                  When a user creates a post, it may contain the identifier of the community
                                  (e.g. hive-174695) or main tag (e.g. travel).
                                  It cannot be modified.

#### Defined in

wasm/lib/proto/comment.ts:27

***

### permlink

> **permlink**: `string`

#### Param

Unique to the author, the identifier of the post or comment.
                           It cannot be modified.

#### Defined in

wasm/lib/proto/comment.ts:37

***

### title

> **title**: `string`

#### Param

The title of the submitted post, in case of the comment, is often empty.
                        It may be modified.

#### Defined in

wasm/lib/proto/comment.ts:42
