[@hiveio/wax](../globals) / transfer\_to\_savings

# Interface: transfer\_to\_savings

A user can place Hive and Hive Dollars into savings balances.
Funds can be withdrawn from these balances after a three day delay.
Keeping funds on the savings balance mitigates loss from hacked and compromised accounts.
The maximum amount a user can lose instantaneously is the sum of what they hold in liquid balances.
Assuming an account can be recovered quickly, loss in such situations can be kept to a minimum
Additionally for keeping Hive Dollars on the savings balance, the interests are calculated.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/32_transfer_to_savings.md?ref_type=heads

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

The allowed currency: HIVE and HBD, amount > 0.

#### Defined in

wasm/lib/proto/transfer\_to\_savings.ts:25

***

### from

> **from**: `string`

#### Param

The account the funds are coming from.

#### Defined in

wasm/lib/proto/transfer\_to\_savings.ts:18

***

### memo

> **memo**: `string`

#### Param

Have to be UTF8, must be shorter than 2048.

#### Defined in

wasm/lib/proto/transfer\_to\_savings.ts:29

***

### to

> **to**: `string`

#### Param

The account the funds are going to.
                             The funds may be transferred to someone else savings balance.

#### Defined in

wasm/lib/proto/transfer\_to\_savings.ts:23
