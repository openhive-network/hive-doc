[@hiveio/wax](../globals) / limit\_order\_create

# Interface: limit\_order\_create

This operation creates a limit order and matches it against existing open orders.
It allows to sell Hive and buy HBD or sell HBD and buy Hive.
It is a way for a user to declare they want to sell {amount_to_sell} Hive/HBD for at least {min_to_receive} HBD/Hive.
The user may be a taker (if a user creates an order and the order matches some order(s))
or a maker (if a user creates an order and the order doesn’t match and the order is waiting for a match on the market).
If there is a partial match, a user may be a taker and maker for the same order.
If a taker creates an order for all orders on the market the order(s) that are the best deal for the taker are matched.
If there are two orders with the same price, the older one is matched.
The operation is used by the markets see: https://wallet.hive.blog/market

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/05_limit_order_create.md?ref_type=heads

## Properties

### amount\_to\_sell

> **amount\_to\_sell**: `undefined` \| [`asset`](./asset)

#### Param

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:25

***

### expiration

> **expiration**: `string`

#### Param

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:39

***

### fill\_or\_kill

> **fill\_or\_kill**: `boolean`

#### Param

If fill_or_kill = true, then the operation is executed immediately or it fails
                             (the operation is not added to the block).
                             If fill_or_kill = false, then the order is valid till 'expiration'.

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:37

***

### min\_to\_receive

> **min\_to\_receive**: `undefined` \| [`asset`](./asset)

#### Param

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:29

***

### orderid

> **orderid**: `number`

#### Param

an ID assigned by owner, must be unique.

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:23

***

### owner

> **owner**: `string`

#### Param

#### Defined in

wasm/lib/proto/limit\_order\_create.ts:21
