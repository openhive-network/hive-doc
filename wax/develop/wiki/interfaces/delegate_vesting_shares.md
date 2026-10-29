[@hiveio/wax](../globals) / delegate\_vesting\_shares

# Interface: delegate\_vesting\_shares

Defined in: wasm/lib/proto/delegate\_vesting\_shares.ts:21

The operation delegate_vesting_shares_operation allows to delegate an amount
of { vesting_shares } to an { delegatee } account. The { vesting_shares } are still owned by { delegator },
but the voting rights and resource credit are transferred.
A user may not delegate:
- the vesting shares that are already delegated
- the delegated vesting shares to him (a user does not own them)
- the vesting shares in the Power down process
- the already used voting shares for voting or downvoting
In order to remove the vesting shares delegation, the operation delegate_vesting_shares_operation
should be created with {vesting_shares = 0}. When a delegation is removed, the delegated vesting shares
are frozen for five days (HIVE_DELEGATION_RETURN_PERIOD_HF20) to prevent voting twice.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/40_delegate_vesting_shares.md?ref_type=heads

## Properties

### delegatee

> **delegatee**: `string`

Defined in: wasm/lib/proto/delegate\_vesting\_shares.ts:25

#### Param

**delegatee**

The account receiving vesting shares.

***

### delegator

> **delegator**: `string`

Defined in: wasm/lib/proto/delegate\_vesting\_shares.ts:23

#### Param

**delegator**

The account delegating vesting shares.

***

### vesting\_shares

> **vesting\_shares**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/delegate\_vesting\_shares.ts:30

#### Param

**vesting\_shares**

The amount of vesting shares to be delegated.
                                Minimal amount = 1/3 of the fee for creating a new account.
