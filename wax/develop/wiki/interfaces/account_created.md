[@hiveio/wax](../globals) / account\_created

# Interface: account\_created

Defined in: wasm/lib/proto/account\_created.ts:12

Related to all acts of account creation, that is, creation of genesis accounts as well as operations:
account_create_operation, account_create_with_delegation_operation, pow_operation, pow2_operation and create_claimed_account_operation.
Generated every time one of above operations results in creation of new account (account is always created except for pow/pow2).
Note: vops for genesis accounts are generated at the start of block #1.

## Properties

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/account\_created.ts:16

#### Param

**creator**

account that initiated new account creation (genesis and mined accounts are their own creators)

***

### initial\_delegation

> **initial\_delegation**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/account\_created.ts:22

#### Param

**initial\_delegation**

(VESTS) amount of extra voting power on new account due to delegation

***

### initial\_vesting\_shares

> **initial\_vesting\_shares**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/account\_created.ts:18

#### Param

**initial\_vesting\_shares**

(VESTS) amount of initial vesting on new account (converted from creation fee prior to HF20)

***

### new\_account\_name

> **new\_account\_name**: `string`

Defined in: wasm/lib/proto/account\_created.ts:14

#### Param

**new\_account\_name**

newly created account (receiver of initial_vesting_shares)
