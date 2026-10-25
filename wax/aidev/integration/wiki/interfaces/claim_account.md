[@hiveio/wax](../globals) / claim\_account

# Interface: claim\_account

A user may create a new account using a pair of operations: claim_account_operation and create_claimed_account_operation.
After the operation claim_account_operation a user receives a token:
pending claimed accounts and later (using operation create_claimed_account_operation) a user may create a new account.
After executing the operation claim_account_operation, a new account is not created.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/22_claim_account.md?ref_type=heads

## Properties

### creator

> **creator**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/claim\_account.ts:17

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

Not currently used.

#### Defined in

wasm/lib/proto/claim\_account.ts:27

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

The amount of fee for creating a new account is decided by the witnesses.
                     It may be paid in HIVE or in the Recourse Credit (RC).
                     If a user wants to pay a fee in RC, it should be set {fee= 0}.

#### Defined in

wasm/lib/proto/claim\_account.ts:23
