[@hiveio/wax](../globals) / transfer\_to\_vesting

# Interface: transfer\_to\_vesting

Defined in: wasm/lib/proto/transfer\_to\_vesting.ts:17

The operation is also called Staking.
This operation converts Hive into Hive Power (also called Vesting Fund Shares  or VESTS) at the current exchange rate.
The conversion may be done between the same account or to another account.
The more HP (Hive Power) the account has, the more:
a.       Governance voting power (for witnesses and proposals) has
b.       Social voting power has (indirectly affects Increase curation rewards)
c.       Resource Credit has

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/03_transfer_to_vesting.md?ref_type=heads

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/transfer\_to\_vesting.ts:23

#### Param

**amount**

Must be HIVE, amount > 0.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/transfer\_to\_vesting.ts:19

#### Param

**from\_account**

The account the funds are coming from.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/transfer\_to\_vesting.ts:21

#### Param

**to\_account**

The account the funds are going to. If null, then the same as 'from_account'.
