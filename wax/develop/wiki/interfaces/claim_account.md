[@hiveio/wax](../globals) / claim\_account

# Interface: claim\_account

Defined in: wasm/lib/proto/claim\_account.ts:15

A user may create a new account using a pair of operations: claim_account_operation and create_claimed_account_operation.
After the operation claim_account_operation a user receives a token:
pending claimed accounts and later (using operation create_claimed_account_operation) a user may create a new account.
After executing the operation claim_account_operation, a new account is not created.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/22_claim_account.md?ref_type=heads

## Properties

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/claim\_account.ts:17

#### Param

**creator**

Account name.

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

Defined in: wasm/lib/proto/claim\_account.ts:27

#### Param

**extensions**

Not currently used.

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/claim\_account.ts:23

#### Param

**fee**

The amount of fee for creating a new account is decided by the witnesses.
                     It may be paid in HIVE or in the Recourse Credit (RC).
                     If a user wants to pay a fee in RC, it should be set {fee= 0}.
