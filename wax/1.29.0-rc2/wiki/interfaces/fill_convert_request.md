[@hiveio/wax](../globals) / fill\_convert\_request

# Interface: fill\_convert\_request

Related to convert_operation.
Generated during block processing after conversion delay passes and HBD is converted to HIVE.

## Properties

### amount\_in

> **amount\_in**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) source of conversion.

#### Defined in

wasm/lib/proto/fill\_convert\_request.ts:16

***

### amount\_out

> **amount\_out**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) effect of conversion.

#### Defined in

wasm/lib/proto/fill\_convert\_request.ts:20

***

### owner

> **owner**: `string`

#### Param

User that requested conversion (receiver of amount_out).

#### Defined in

wasm/lib/proto/fill\_convert\_request.ts:12

***

### requestid

> **requestid**: `number`

#### Param

id of the request.

#### Defined in

wasm/lib/proto/fill\_convert\_request.ts:14
