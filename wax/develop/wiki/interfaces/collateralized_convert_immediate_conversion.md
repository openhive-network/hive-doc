[@hiveio/wax](../globals) / collateralized\_convert\_immediate\_conversion

# Interface: collateralized\_convert\_immediate\_conversion

Defined in: wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:11

Related to collateralized_convert_operation.
Generated every time above operation is executed. Contains amount of HBD received right when the transfer actually happens.

## See

fill_collateralized_convert_request

## Properties

### hbd\_out

> **hbd\_out**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:17

#### Param

**hbd\_out**

(HBD) funds after conversion

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:13

#### Param

**owner**

user that requested conversion (receiver of hbd_out)

***

### requestid

> **requestid**: `number`

Defined in: wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:15

#### Param

**requested**

id of the conversion request
