[@hiveio/wax](../globals) / account\_update

# Interface: account\_update

Defined in: wasm/lib/proto/account\_update.ts:14

Operations account_update_operation and account_update2_operation share a limit of allowed updates of the owner authority:
two executions per 60 minutes (HIVE_OWNER_UPDATE_LIMIT) (meaning each of them can be executed twice or both can be executed once during that time period).
After 30 days (HIVE_OWNER_AUTH_RECOVERY_PERIOD) using the account recovery process to change the owner authority is no longer possible.
The operation account_update_operation allows changing authorities, it doesn't allow changing the posting_json_metadata.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/10_account_update.md?ref_type=heads

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/account\_update.ts:16

#### Param

**account**

Account name, it cannot be updated.

***

### active?

> `optional` **active?**: [`authority`](./authority)

Defined in: wasm/lib/proto/account\_update.ts:30

#### Param

**active**

In order to update the {active}, the active authority is required.
                            If a user provides a new authority, the old one will be deleted.

***

### json\_metadata

> **json\_metadata**: `string`

Defined in: wasm/lib/proto/account\_update.ts:46

#### Param

**json\_metadata**

json_string; in order to update the {json_metadata}, the active authority is required.

***

### memo\_key

> **memo\_key**: `string`

Defined in: wasm/lib/proto/account\_update.ts:44

#### Param

**memo\_key**

In order to update the {memo_key}, active authority is required.
                           If a user provides a new key, the old one will be deleted.

***

### owner?

> `optional` **owner?**: [`authority`](./authority)

Defined in: wasm/lib/proto/account\_update.ts:23

#### Param

**owner**

In order to update the {owner}, the owner authority is required.
                           It may be changed 2 times per hour.
                           If a user provides a new authority, the old one will be deleted,
                           but the deleted authority may be used up to 30 days in the process of the recovery account.

***

### posting?

> `optional` **posting?**: [`authority`](./authority)

Defined in: wasm/lib/proto/account\_update.ts:37

#### Param

**posting**

In order to update the {posting}, the active authority is required.
                             If a user provides a new authority, the old one will be deleted.
