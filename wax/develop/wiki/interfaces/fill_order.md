[@hiveio/wax](../globals) / fill\_order

# Interface: fill\_order

Related to limit_order_create_operation and limit_order_create2_operation.
Generated during one of above operations when order on internal market is partially or fully matched
(each match generates separate vop).

## Properties

### current\_orderid

> **current\_orderid**: `number`

#### Param

id of fresh order

#### Defined in

wasm/lib/proto/fill\_order.ts:15

***

### current\_owner

> **current\_owner**: `string`

#### Param

user that recently created order (taker - receiver of open_pays)

#### Defined in

wasm/lib/proto/fill\_order.ts:13

***

### current\_pays

> **current\_pays**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE or HBD) amount paid to open_owner

#### Defined in

wasm/lib/proto/fill\_order.ts:17

***

### open\_orderid

> **open\_orderid**: `number`

#### Param

id of waiting order

#### Defined in

wasm/lib/proto/fill\_order.ts:23

***

### open\_owner

> **open\_owner**: `string`

#### Param

user that had his order on the market (maker - receiver of current_pays)

#### Defined in

wasm/lib/proto/fill\_order.ts:21

***

### open\_pays

> **open\_pays**: `undefined` \| [`asset`](./asset)

#### Param

(HBD or HIVE) amount paid to current_owner

#### Defined in

wasm/lib/proto/fill\_order.ts:25
