[@hiveio/wax](../globals) / limit\_order\_cancel

# Interface: limit\_order\_cancel

Defined in: wasm/lib/proto/limit\_order\_cancel.ts:11

Cancels an order (limit_order_create_operation or limit_order_create2_operation)
and returns the balance to the owner.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/06_limit_order_cancel.md?ref_type=heads

## Properties

### orderid

> **orderid**: `number`

Defined in: wasm/lib/proto/limit\_order\_cancel.ts:18

#### Param

**orderid**

The request_id provided by a user during creating a limit_order_create_operation
                          or limit_order_create2_operation.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/limit\_order\_cancel.ts:13

#### Param

**owner**
