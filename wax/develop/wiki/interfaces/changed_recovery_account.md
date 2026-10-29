[@hiveio/wax](../globals) / changed\_recovery\_account

# Interface: changed\_recovery\_account

Defined in: wasm/lib/proto/changed\_recovery\_account.ts:9

Related to change_recovery_account_operation.
Generated during block processing after wait period for the recovery account change has passed and the change became active.

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/changed\_recovery\_account.ts:11

#### Param

**account**

used that requested recovery accout change

***

### new\_recovery\_account

> **new\_recovery\_account**: `string`

Defined in: wasm/lib/proto/changed\_recovery\_account.ts:15

#### Param

**new\_recovery\_account**

new recovery account

***

### old\_recovery\_account

> **old\_recovery\_account**: `string`

Defined in: wasm/lib/proto/changed\_recovery\_account.ts:13

#### Param

**old\_recovery\_account**

previous recovery account
