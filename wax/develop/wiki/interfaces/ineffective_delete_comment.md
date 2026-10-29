[@hiveio/wax](../globals) / ineffective\_delete\_comment

# Interface: ineffective\_delete\_comment

Defined in: wasm/lib/proto/ineffective\_delete\_comment.ts:11

Related to delete_comment_operation.
Generated when delete_comment_operation was executed but ignored.
Note: prior to HF19 it was possible to execute delete on comment that had net positive votes. Such operation was ignored.
This is the moment this vop is generated.

## Properties

### author

> **author**: `string`

Defined in: wasm/lib/proto/ineffective\_delete\_comment.ts:13

#### Param

**author**

author of attempted-delete comment

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/ineffective\_delete\_comment.ts:15

#### Param

**permlink**

permlink of attempted-delete comment
