[@hiveio/wax](../globals) / collateralized\_convert\_immediate\_conversion

# Interface: collateralized\_convert\_immediate\_conversion

Related to collateralized_convert_operation.
Generated every time above operation is executed. Contains amount of HBD received right when the transfer actually happens.

## See

fill_collateralized_convert_request

## Properties

### hbd\_out

> **hbd\_out**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) funds after conversion

#### Defined in

wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:17

***

### owner

> **owner**: `string`

#### Param

user that requested conversion (receiver of hbd_out)

#### Defined in

wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:13

***

### requestid

> **requestid**: `number`

#### Param

id of the conversion request

#### Defined in

wasm/lib/proto/collateralized\_convert\_immediate\_conversion.ts:15
