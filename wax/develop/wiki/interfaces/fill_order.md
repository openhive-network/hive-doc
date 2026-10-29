[@hiveio/wax](../globals) / fill\_order

# Interface: fill\_order

Defined in: wasm/lib/proto/fill\_order.ts:11

Related to limit_order_create_operation and limit_order_create2_operation.
Generated during one of above operations when order on internal market is partially or fully matched
(each match generates separate vop).

## Properties

### current\_orderid

> **current\_orderid**: `number`

Defined in: wasm/lib/proto/fill\_order.ts:15

#### Param

**current\_orderid**

id of fresh order

***

### current\_owner

> **current\_owner**: `string`

Defined in: wasm/lib/proto/fill\_order.ts:13

#### Param

**current\_owner**

user that recently created order (taker - receiver of open_pays)

***

### current\_pays

> **current\_pays**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_order.ts:17

#### Param

**current\_pays**

(HIVE or HBD) amount paid to open_owner

***

### open\_orderid

> **open\_orderid**: `number`

Defined in: wasm/lib/proto/fill\_order.ts:23

#### Param

**open\_orderid**

id of waiting order

***

### open\_owner

> **open\_owner**: `string`

Defined in: wasm/lib/proto/fill\_order.ts:21

#### Param

**open\_owner**

user that had his order on the market (maker - receiver of current_pays)

***

### open\_pays

> **open\_pays**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_order.ts:25

#### Param

**open\_pays**

(HBD or HIVE) amount paid to current_owner
