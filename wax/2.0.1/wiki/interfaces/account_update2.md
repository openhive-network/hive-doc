[@hiveio/wax](../globals) / account\_update2

# Interface: account\_update2

There are two operations that allow updating an account data: account_update_operation and account_update2_operation.
Operations account_update_operation and account_update2_operation share a limit of allowed updates
of the owner authority  - two executions per 60 minutes (HIVE_OWNER_UPDATE_LIMIT) - meaning each of them
can be executed twice or both can be executed once during that time period.
After 30 days (HIVE_OWNER_AUTH_RECOVERY_PERIOD) using the account recovery process to change the owner authority is no longer possible.
The operation allows to update authority, json_metadata and the posting_json_metadata.
Depending on what the user wants to change, a different authority has to be used.
Each authority (owner, active, posting, memo_key) consists of:
- weight_threshold
- key or account name with its weight
The authority may have more than one key and more than one assigned account name.

## Examples

```ts
Example 1:
The posting authority:
weight_threshold = 1
'first_key', weight = 1
'second_key', weight = 1
'account_name_1', weight = 1
The above settings mean that a user with 'first_key', a user with 'second_key' or a user 'account_name_1'
may post on behalf of this account.
```

```ts
Example 2:
The posting authority:
weight_threshold = 2
'first_key', weight = 1
'second_key', weight = 1
'account_name_1', weight = 1
The above settings mean that at least two signatures are needed to post on behalf of this account.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/43_account_update2.md?ref_type=heads
```

## Properties

### account

> **account**: `string`

#### Param

Account name, it cannot be updated.

#### Defined in

wasm/lib/proto/account\_update2.ts:41

***

### active?

> `optional` **active**: [`authority`](./authority)

#### Param

Optional. In order to update the {active}, the active authority is required.
                            If a user provides a new authority, the old one will be deleted.

#### Defined in

wasm/lib/proto/account\_update2.ts:54

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

#### Defined in

wasm/lib/proto/account\_update2.ts:79

***

### json\_metadata

> **json\_metadata**: `string`

#### Param

json_string; In order to update the {json_metadata}, the active authority is required.

#### Defined in

wasm/lib/proto/account\_update2.ts:72

***

### memo\_key?

> `optional` **memo\_key**: `string`

#### Param

Optional. In order to update the {memo_key}, the active authority is required.
                           If a user provides a new key, the old one will be deleted.

#### Defined in

wasm/lib/proto/account\_update2.ts:68

***

### owner?

> `optional` **owner**: [`authority`](./authority)

#### Param

Optional. In order to update the {owner}, the owner authority is required.
                           It may be changed 2 times per hour.
                           If a user provides a new authority, the old one will be deleted.

#### Defined in

wasm/lib/proto/account\_update2.ts:47

***

### posting?

> `optional` **posting**: [`authority`](./authority)

#### Param

Optional. In order to update the {posting}, the active authority is required.
                             If a user provides a new authority, the old one will be deleted.

#### Defined in

wasm/lib/proto/account\_update2.ts:61

***

### posting\_json\_metadata

> **posting\_json\_metadata**: `string`

#### Param

json_string; In order to update the { posting_json_metadata },
                                        the posting authority is required.

#### Defined in

wasm/lib/proto/account\_update2.ts:77
