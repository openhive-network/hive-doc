[@hiveio/wax](../globals) / withdraw\_vesting

# Interface: withdraw\_vesting

This operation converts Hive Power (also called Vesting Fund Shares or VESTS) into HIVE.
At any given point in time an account can be withdrawing from their vesting shares.
A user may change the number of shares they wish to cash out at any time between 0 and their total vesting stake.
After applying this operation, vesting_shares will be withdrawn at a rate of vesting_shares/13 per week for 13 weeks
starting one week after this operation is included in the blockchain.
This operation is not valid if a user has no vesting shares.
There can be only one withdraw_vesting_operation  processed at the same time.
If a user wants to stop withdraw_vesting_operation, they should create an operation withdraw_vesting_operation with amount =0.
If a user creates a new withdraw_vesting_operation when the old one is still processed,
then the old withdraw_vesting_operation will be canceled and a new one will be processed.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/04_withdraw_vesting.md?ref_type=heads

## Properties

### account

> **account**: `string`

#### Param

The account the funds are coming from.

#### Defined in

wasm/lib/proto/withdraw\_vesting.ts:22

***

### vesting\_shares

> **vesting\_shares**: `undefined` \| [`asset`](./asset)

#### Param

Amount of VESTS (HP)

#### Defined in

wasm/lib/proto/withdraw\_vesting.ts:24
