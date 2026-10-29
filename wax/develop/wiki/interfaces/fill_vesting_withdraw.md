[@hiveio/wax](../globals) / fill\_vesting\_withdraw

# Interface: fill\_vesting\_withdraw

Defined in: wasm/lib/proto/fill\_vesting\_withdraw.ts:12

Related to withdraw_vesting_operation and set_withdraw_vesting_route_operation.
Generated during block processing in batches for each active withdraw route (including implied
from_account(VESTS)->from_account(HIVE)) each time vesting withdrawal period passes.
Note: not generated for implied route when all funds were already distributed along explicit routes

## Properties

### deposited

> **deposited**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_vesting\_withdraw.ts:22

#### Param

**deposited**

(HIVE or VESTS) [converted] target amount

***

### from\_account

> **from\_account**: `string`

Defined in: wasm/lib/proto/fill\_vesting\_withdraw.ts:14

#### Param

**from\_account**

user that activated power down

***

### to\_account

> **to\_account**: `string`

Defined in: wasm/lib/proto/fill\_vesting\_withdraw.ts:16

#### Param

**to\_account**

target of vesting route (potentially the same as from_account - receiver of deposited)

***

### withdrawn

> **withdrawn**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_vesting\_withdraw.ts:18

#### Param

**withdraw**

(VESTS) source amount
