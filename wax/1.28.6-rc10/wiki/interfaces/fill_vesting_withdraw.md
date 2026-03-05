[@hiveio/wax](../globals) / fill\_vesting\_withdraw

# Interface: fill\_vesting\_withdraw

Related to withdraw_vesting_operation and set_withdraw_vesting_route_operation.
Generated during block processing in batches for each active withdraw route (including implied
from_account(VESTS)->from_account(HIVE)) each time vesting withdrawal period passes.
Note: not generated for implied route when all funds were already distributed along explicit routes

## Properties

### deposited

> **deposited**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE or VESTS) [converted] target amount

#### Defined in

wasm/lib/proto/fill\_vesting\_withdraw.ts:22

***

### from\_account

> **from\_account**: `string`

#### Param

user that activated power down

#### Defined in

wasm/lib/proto/fill\_vesting\_withdraw.ts:14

***

### to\_account

> **to\_account**: `string`

#### Param

target of vesting route (potentially the same as from_account - receiver of deposited)

#### Defined in

wasm/lib/proto/fill\_vesting\_withdraw.ts:16

***

### withdrawn

> **withdrawn**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) source amount

#### Defined in

wasm/lib/proto/fill\_vesting\_withdraw.ts:18
