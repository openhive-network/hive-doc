[@hiveio/wax](../globals) / limit\_order\_cancelled

# Interface: limit\_order\_cancelled

Defined in: wasm/lib/proto/limit\_order\_cancelled.ts:13

Related to limit_order_cancel_operation, limit_order_create_operation or limit_order_create2_operation.
Generated every time existing limit order is cancelled. It happens on explicit call (first operation), or in rare case of
filling limit order (second or third operation) when, after filling most of it, remaining funds are too small (would round
to zero when sold). Finally also generated during block processing for orders that reached expiration time without being filled.

## See

fill_order

## Properties

### amount\_back

> **amount\_back**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/limit\_order\_cancelled.ts:19

#### Param

**amount\_back**

(HIVE or HBD) remaining funds from original order that were not traded until cancellation

***

### orderid

> **orderid**: `number`

Defined in: wasm/lib/proto/limit\_order\_cancelled.ts:17

#### Param

**orderid**

id of the order

***

### seller

> **seller**: `string`

Defined in: wasm/lib/proto/limit\_order\_cancelled.ts:15

#### Param

**seller**

user that placed an order (receiver of amount_back)
