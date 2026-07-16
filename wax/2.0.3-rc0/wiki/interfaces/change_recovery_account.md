[@hiveio/wax](../globals) / change\_recovery\_account

# Interface: change\_recovery\_account

The operation change_recovery_account_operation allows a user to update their recovery account.
It is important to keep it actual, because only a recovery account may create a request
account recovery in case of compromised the owner authority.
By default the recovery account is set to the account creator or it is empty if it was created by temp account or mined.
In order to cancel the change_recovery_account_operation, the operation change_recovery_account_operation,
the operation should be created with {new_recovery_account} set to the old one.
The operation is done with a 30 days (HIVE_OWNER_AUTH_RECOVERY_PERIOD) delay.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/26_change_recovery_account.md?ref_type=heads

## Properties

### account\_to\_recover

> **account\_to\_recover**: `string`

#### Param

#### Defined in

wasm/lib/proto/change\_recovery\_account.ts:19

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

#### Defined in

wasm/lib/proto/change\_recovery\_account.ts:23

***

### new\_recovery\_account

> **new\_recovery\_account**: `string`

#### Param

#### Defined in

wasm/lib/proto/change\_recovery\_account.ts:21
