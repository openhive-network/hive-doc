[@hiveio/wax](../globals) / set\_withdraw\_vesting\_route

# Interface: set\_withdraw\_vesting\_route

The operation set_withdraw_vesting_route_operation allows a user to decide where
and how much percent of hive should be transferred to  the account { to_account }
from power down operation. A user may also decide that the Hive may be immediately converted to Hive Power.
The operation may be created in any moment of power down operation and even if there is no power down operation in progress.
The setting is valid till a user creates an operation  set_withdraw_vesting_route_operation
with the same { to_account} and with the {percent} = 0.
A user may set up 10 { to_account } accounts.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/20_set_withdraw_vesting_route.md?ref_type=heads

## Properties

### auto\_vest

> **auto\_vest**: `boolean`

#### Param

If auto_vest = true, then the amount of the Hive is immediately converted
                          into HP on the { to_account } balance.
                          If auto_vest = false, there is no conversion from Hive into HP.
                          Default auto_vest = false;

#### Defined in

wasm/lib/proto/set\_withdraw\_vesting\_route.ts:34

***

### from\_account

> **from\_account**: `string`

#### Param

The account the funds are coming from.

#### Defined in

wasm/lib/proto/set\_withdraw\_vesting\_route.ts:18

***

### percent

> **percent**: `number`

#### Param

The percentage of the HP shares.
                          If the sum of the setting shares is less than 100%,
                          the rest is transferred to the liquid balance of { from_account }.
                          Default value: percent = 0;

#### Defined in

wasm/lib/proto/set\_withdraw\_vesting\_route.ts:27

***

### to\_account

> **to\_account**: `string`

#### Param

The account the funds are going to. A user may set up 10 accounts.

#### Defined in

wasm/lib/proto/set\_withdraw\_vesting\_route.ts:20
