[@hiveio/wax](../globals) / fill\_transfer\_from\_savings

# Interface: fill\_transfer\_from\_savings

Related to transfer_from_savings_operation.
Generated during block processing after savings withdraw time has passed and requested amount
was transfered from savings to liquid balance.

## Properties

### amount

> **amount**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE or HBD) funds transfered from savings

#### Defined in

wasm/lib/proto/fill\_transfer\_from\_savings.ts:17

***

### from

> **from**: `string`

#### Param

user that initiated transfer from savings

#### Defined in

wasm/lib/proto/fill\_transfer\_from\_savings.ts:13

***

### memo

> **memo**: `string`

#### Param

memo attached to transfer request

#### Defined in

wasm/lib/proto/fill\_transfer\_from\_savings.ts:23

***

### request\_id

> **request\_id**: `number`

#### Param

id of transfer request

#### Defined in

wasm/lib/proto/fill\_transfer\_from\_savings.ts:21

***

### to

> **to**: `string`

#### Param

user that was specified to receive funds (receiver of amount)

#### Defined in

wasm/lib/proto/fill\_transfer\_from\_savings.ts:15
