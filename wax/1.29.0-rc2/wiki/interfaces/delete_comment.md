[@hiveio/wax](../globals) / delete\_comment

# Interface: delete\_comment

The post or comment may be deleted by the author. If the post or comment is deleted, the {permlink} may be reused.
The delete doesn’t mean that the comment is removed from the blockchain.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/17_delete_comment.md?ref_type=heads

## Properties

### author

> **author**: `string`

#### Param

Account name, the author of the post or the comment.

#### Defined in

wasm/lib/proto/delete\_comment.ts:13

***

### permlink

> **permlink**: `string`

#### Param

The identifier of the post or the comment.

#### Defined in

wasm/lib/proto/delete\_comment.ts:15
