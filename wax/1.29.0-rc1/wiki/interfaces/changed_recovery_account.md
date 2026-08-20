[@hiveio/wax](../globals) / changed\_recovery\_account

# Interface: changed\_recovery\_account

Related to change_recovery_account_operation.
Generated during block processing after wait period for the recovery account change has passed and the change became active.

## Properties

### account

> **account**: `string`

#### Param

used that requested recovery accout change

#### Defined in

wasm/lib/proto/changed\_recovery\_account.ts:11

***

### new\_recovery\_account

> **new\_recovery\_account**: `string`

#### Param

new recovery account

#### Defined in

wasm/lib/proto/changed\_recovery\_account.ts:15

***

### old\_recovery\_account

> **old\_recovery\_account**: `string`

#### Param

previous recovery account

#### Defined in

wasm/lib/proto/changed\_recovery\_account.ts:13
