[@hiveio/wax](../globals) / limit\_order\_create2

# Interface: limit\_order\_create2

Defined in: wasm/lib/proto/limit\_order\_create2.ts:15

This operation creates a limit order and matches it against existing open orders.
It is similar to limit_order_create except it serializes the price rather than calculating it from other fields.
It allows to sell Hive and buy HBD or sell HBD and buy Hive.
It is a way for a user to declare they wants to sell {amount_to_sell} Hive/HBD for at least {exchange_rate}  per HBD/Hive.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/21_limit_order_create2.md?ref_type=heads

## Properties

### amount\_to\_sell

> **amount\_to\_sell**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:21

#### Param

**amount\_to\_sell**

***

### exchange\_rate

> **exchange\_rate**: [`price`](./price) \| `undefined`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:31

#### Param

**exchange\_rate**

***

### expiration

> **expiration**: `string`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:35

#### Param

**expiration**

***

### fill\_or\_kill

> **fill\_or\_kill**: `boolean`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:29

#### Param

**fill\_or\_kill**

If fill_or_kill = true, then the operation is executed immediately
                             or it fails (the operation is not added to the block).
                             If fill_or_kill = false, then the order is valid till {expiration}.

***

### orderid

> **orderid**: `number`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:19

#### Param

**orderid**

an ID assigned by owner, must be unique.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/limit\_order\_create2.ts:17

#### Param

**owner**
