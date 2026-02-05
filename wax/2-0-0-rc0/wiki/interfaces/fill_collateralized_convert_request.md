[@hiveio/wax](../globals) / fill\_collateralized\_convert\_request

# Interface: fill\_collateralized\_convert\_request

Related to collateralized_convert_operation.
Generated during block processing after conversion delay passes and HIVE is finally converted to HBD.
Note: HBD is transferred immediately during execution of above operation, this vop is generated after actual
price of conversion becomes known.

## See

collateralized_convert_immediate_conversion

## Properties

### amount\_in

> **amount\_in**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) source of conversion (part of collateral)

#### Defined in

wasm/lib/proto/fill\_collateralized\_convert\_request.ts:19

***

### amount\_out

> **amount\_out**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) result of conversion (already transferred to owner when request was made)

#### Defined in

wasm/lib/proto/fill\_collateralized\_convert\_request.ts:23

***

### excess\_collateral

> **excess\_collateral**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) unused part of collateral returned to owner

#### Defined in

wasm/lib/proto/fill\_collateralized\_convert\_request.ts:27

***

### owner

> **owner**: `string`

#### Param

user that requested conversion (receiver of excess_collateral)

#### Defined in

wasm/lib/proto/fill\_collateralized\_convert\_request.ts:15

***

### requestid

> **requestid**: `number`

#### Param

id of the request

#### Defined in

wasm/lib/proto/fill\_collateralized\_convert\_request.ts:17
