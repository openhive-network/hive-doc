[@hiveio/wax](../globals) / fill\_convert\_request

# Interface: fill\_convert\_request

Defined in: wasm/lib/proto/fill\_convert\_request.ts:10

Related to convert_operation.
Generated during block processing after conversion delay passes and HBD is converted to HIVE.

## Properties

### amount\_in

> **amount\_in**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_convert\_request.ts:16

#### Param

**amount\_in**

(HBD) source of conversion.

***

### amount\_out

> **amount\_out**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/fill\_convert\_request.ts:20

#### Param

**amount\_out**

(HIVE) effect of conversion.

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/fill\_convert\_request.ts:12

#### Param

**owner**

User that requested conversion (receiver of amount_out).

***

### requestid

> **requestid**: `number`

Defined in: wasm/lib/proto/fill\_convert\_request.ts:14

#### Param

**requestid**

id of the request.
