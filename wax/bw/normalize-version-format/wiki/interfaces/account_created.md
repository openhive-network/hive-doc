[@hiveio/wax](../globals) / account\_created

# Interface: account\_created

Related to all acts of account creation, that is, creation of genesis accounts as well as operations:
account_create_operation, account_create_with_delegation_operation, pow_operation, pow2_operation and create_claimed_account_operation.
Generated every time one of above operations results in creation of new account (account is always created except for pow/pow2).
Note: vops for genesis accounts are generated at the start of block #1.

## Properties

### creator

> **creator**: `string`

#### Param

account that initiated new account creation (genesis and mined accounts are their own creators)

#### Defined in

wasm/lib/proto/account\_created.ts:16

***

### initial\_delegation

> **initial\_delegation**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) amount of extra voting power on new account due to delegation

#### Defined in

wasm/lib/proto/account\_created.ts:22

***

### initial\_vesting\_shares

> **initial\_vesting\_shares**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) amount of initial vesting on new account (converted from creation fee prior to HF20)

#### Defined in

wasm/lib/proto/account\_created.ts:18

***

### new\_account\_name

> **new\_account\_name**: `string`

#### Param

newly created account (receiver of initial_vesting_shares)

#### Defined in

wasm/lib/proto/account\_created.ts:14
