[@hiveio/wax](../globals) / limit\_order\_create

# Interface: limit\_order\_create

Defined in: wasm/lib/proto/limit\_order\_create.ts:19

This operation creates a limit order and matches it against existing open orders.
It allows to sell Hive and buy HBD or sell HBD and buy Hive.
It is a way for a user to declare they want to sell {amount_to_sell} Hive/HBD for at least {min_to_receive} HBD/Hive.
The user may be a taker (if a user creates an order and the order matches some order(s))
or a maker (if a user creates an order and the order doesn't match and the order is waiting for a match on the market).
If there is a partial match, a user may be a taker and maker for the same order.
If a taker creates an order for all orders on the market the order(s) that are the best deal for the taker are matched.
If there are two orders with the same price, the older one is matched.
The operation is used by the markets see: https://wallet.hive.blog/market

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/05_limit_order_create.md?ref_type=heads

## Properties

### amount\_to\_sell

> **amount\_to\_sell**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/limit\_order\_create.ts:25

#### Param

**amount\_to\_sell**

***

### expiration

> **expiration**: `string`

Defined in: wasm/lib/proto/limit\_order\_create.ts:39

#### Param

**expiration**

***

### fill\_or\_kill

> **fill\_or\_kill**: `boolean`

Defined in: wasm/lib/proto/limit\_order\_create.ts:37

#### Param

**fill\_or\_kill**

If fill_or_kill = true, then the operation is executed immediately or it fails
                             (the operation is not added to the block).
                             If fill_or_kill = false, then the order is valid till 'expiration'.

***

### min\_to\_receive

> **min\_to\_receive**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/limit\_order\_create.ts:29

#### Param

**min\_to\_receive**

***

### orderid

> **orderid**: `number`

Defined in: wasm/lib/proto/limit\_order\_create.ts:23

#### Param

**orderid**

an ID assigned by owner, must be unique.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/limit\_order\_create.ts:21

#### Param

**owner**
