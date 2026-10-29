[@hiveio/wax](../globals) / fill\_transfer\_from\_savings

# Interface: fill\_transfer\_from\_savings

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:11

Related to transfer_from_savings_operation.
Generated during block processing after savings withdraw time has passed and requested amount
was transfered from savings to liquid balance.

## Properties

### amount

> **amount**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:17

#### Param

**amount**

(HIVE or HBD) funds transfered from savings

***

### from

> **from**: `string`

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:13

#### Param

**from\_account**

user that initiated transfer from savings

***

### memo

> **memo**: `string`

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:23

#### Param

**memo**

memo attached to transfer request

***

### request\_id

> **request\_id**: `number`

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:21

#### Param

**request\_id**

id of transfer request

***

### to

> **to**: `string`

Defined in: wasm/lib/proto/fill\_transfer\_from\_savings.ts:15

#### Param

**to\_account**

user that was specified to receive funds (receiver of amount)
