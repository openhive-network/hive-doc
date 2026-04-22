[@hiveio/wax](../globals) / limit\_order\_cancelled

# Interface: limit\_order\_cancelled

Related to limit_order_cancel_operation, limit_order_create_operation or limit_order_create2_operation.
Generated every time existing limit order is cancelled. It happens on explicit call (first operation), or in rare case of
filling limit order (second or third operation) when, after filling most of it, remaining funds are too small (would round
to zero when sold). Finally also generated during block processing for orders that reached expiration time without being filled.

## See

fill_order

## Properties

### amount\_back

> **amount\_back**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE or HBD) remaining funds from original order that were not traded until cancellation

#### Defined in

wasm/lib/proto/limit\_order\_cancelled.ts:19

***

### orderid

> **orderid**: `number`

#### Param

id of the order

#### Defined in

wasm/lib/proto/limit\_order\_cancelled.ts:17

***

### seller

> **seller**: `string`

#### Param

user that placed an order (receiver of amount_back)

#### Defined in

wasm/lib/proto/limit\_order\_cancelled.ts:15
