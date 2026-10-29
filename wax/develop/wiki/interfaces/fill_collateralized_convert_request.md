[@hiveio/wax](../globals) / fill\_collateralized\_convert\_request

# Interface: fill\_collateralized\_convert\_request

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:13

Related to collateralized_convert_operation.
Generated during block processing after conversion delay passes and HIVE is finally converted to HBD.
Note: HBD is transferred immediately during execution of above operation, this vop is generated after actual
price of conversion becomes known.

## See

collateralized_convert_immediate_conversion

## Properties

### amount\_in

> **amount\_in**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:19

#### Param

**amount\_in**

(HIVE) source of conversion (part of collateral)

***

### amount\_out

> **amount\_out**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:23

#### Param

**amount\_out**

(HBD) result of conversion (already transferred to owner when request was made)

***

### excess\_collateral

> **excess\_collateral**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:27

#### Param

**excess\_collateral**

(HIVE) unused part of collateral returned to owner

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:15

#### Param

**owner**

user that requested conversion (receiver of excess_collateral)

***

### requestid

> **requestid**: `number`

Defined in: wasm/lib/proto/fill\_collateralized\_convert\_request.ts:17

#### Param

**requestid**

id of the request
