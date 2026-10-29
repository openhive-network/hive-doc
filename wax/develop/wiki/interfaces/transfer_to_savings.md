[@hiveio/wax](../globals) / transfer\_to\_savings

# Interface: transfer\_to\_savings

Defined in: wasm/lib/proto/transfer\_to\_savings.ts:16

A user can place Hive and Hive Dollars into savings balances.
Funds can be withdrawn from these balances after a three day delay.
Keeping funds on the savings balance mitigates loss from hacked and compromised accounts.
The maximum amount a user can lose instantaneously is the sum of what they hold in liquid balances.
Assuming an account can be recovered quickly, loss in such situations can be kept to a minimum
Additionally for keeping Hive Dollars on the savings balance, the interests are calculated.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/32_transfer_to_savings.md?ref_type=heads

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/transfer\_to\_savings.ts:25

#### Param

**amount**

The allowed currency: HIVE and HBD, amount > 0.

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/transfer\_to\_savings.ts:18

#### Param

**from\_account**

The account the funds are coming from.

***

### memo

> **memo**: `string`

Defined in: wasm/lib/proto/transfer\_to\_savings.ts:29

#### Param

**memo**

Have to be UTF8, must be shorter than 2048.

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/transfer\_to\_savings.ts:23

#### Param

**to\_account**

The account the funds are going to.
                             The funds may be transferred to someone else savings balance.
