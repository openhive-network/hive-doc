[@hiveio/wax](../globals) / recover\_account

# Interface: recover\_account

Defined in: wasm/lib/proto/recover\_account.ts:18

This operation is part of the recovery account process (more information in request_account_recovery).
After creating by recovery account the operation request_account_recovery,
the user has HIVE_ACCOUNT_RECOVERY_REQUEST_EXPIRATION_PERIOD hours to respond using
operation recover_account_operation and set a new owner authority.
The operation recover_account_operation has to be signed using the two owner authorities,
the old one (maybe compromised) and the new one (see request_account_recovery).
There must be at least 60 minutes (HIVE_OWNER_UPDATE_LIMIT) between executions of operation recover_account_operation.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/25_recover_account.md?ref_type=heads

## Properties

### account\_to\_recover

> **account\_to\_recover**: `string`

Defined in: wasm/lib/proto/recover\_account.ts:20

#### Param

**account\_to\_recover**

The account to be recovered.

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

Defined in: wasm/lib/proto/recover\_account.ts:34

#### Param

**extensions**

Not currently used.

***

### new\_owner\_authority

> **new\_owner\_authority**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/recover\_account.ts:22

#### Param

**new\_owner\_authority**

The new owner authority as specified in the request account recovery operation.

***

### recent\_owner\_authority

> **recent\_owner\_authority**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/recover\_account.ts:30

#### Param

**recent\_owner\_authority**

A previous owner's authority, may be compromised.
                                            If the operation change_recovery_account_operation was generated,
                                            it has not been yet 30 days since its creation.
