[@hiveio/wax](../globals) / custom\_json

# Variable: custom\_json

> **custom\_json**: `object`

## Type declaration

### create()

#### Type Parameters

• **I** *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### base?

`I`

#### Returns

[`custom_json`](../interfaces/custom_json)

### fromJSON()

#### Parameters

##### object

`any`

#### Returns

[`custom_json`](../interfaces/custom_json)

### fromPartial()

#### Type Parameters

• **I** *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### object

`I`

#### Returns

[`custom_json`](../interfaces/custom_json)

### toJSON()

#### Parameters

##### message

[`custom_json`](../interfaces/custom_json)

#### Returns

`unknown`

## Defined in

wasm/lib/proto/custom\_json.ts:18
