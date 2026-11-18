[@hiveio/wax](../globals) / delegate\_rc

# Interface: delegate\_rc

Defined in: wasm/lib/proto/delegate\_rc.ts:17

The operation delegate_rc_operation sets the amount of resource credits (RC) that { from } delegates
to each account listed in { delegatees }. Only RC is delegated - the vesting shares (HP), their voting power
and governance rights stay with { from }. If there is no delegation yet, a new one is created, if there is,
it is increased or decreased to { max_rc }; { max_rc } = 0 removes the delegation.
Since HF 26 the operation can be embedded in custom_json_operation with id "rc", since HF 29 it can also be
used as a regular operation. Account history shows effective embedded delegations as delegate_rc_operation
placed right after their custom_json_operation.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/37_delegate_rc.md?ref_type=heads

## Properties

### delegatees

> **delegatees**: `string`[]

Defined in: wasm/lib/proto/delegate\_rc.ts:21

#### Param

**delegatees**

Accounts receiving RC (up to 100, without { from }).

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

Defined in: wasm/lib/proto/delegate\_rc.ts:28

#### Param

**extensions**

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/delegate\_rc.ts:19

#### Param

**from\_account**

The account delegating RC.

***

### max\_rc

> **max\_rc**: `string`

Defined in: wasm/lib/proto/delegate\_rc.ts:26

#### Param

**max\_rc**

The amount of RC delegated to each of { delegatees }. 0 removes the delegation.
                         Otherwise it has to be at least 1/3 of the fee for creating a new account (expressed in VESTS).
