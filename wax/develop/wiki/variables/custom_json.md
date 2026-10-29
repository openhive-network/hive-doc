[@hiveio/wax](../globals) / custom\_json

# Variable: custom\_json

> **custom\_json**: `object`

Defined in: wasm/lib/proto/custom\_json.ts:18

## Type Declaration

### create()

> **create**\<`I`\>(`base?`): [`custom_json`](../interfaces/custom_json)

#### Type Parameters

##### I

`I` *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### base?

`I`

#### Returns

[`custom_json`](../interfaces/custom_json)

### fromJSON()

> **fromJSON**(`object`): [`custom_json`](../interfaces/custom_json)

#### Parameters

##### object

`any`

#### Returns

[`custom_json`](../interfaces/custom_json)

### fromPartial()

> **fromPartial**\<`I`\>(`object`): [`custom_json`](../interfaces/custom_json)

#### Type Parameters

##### I

`I` *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### object

`I`

#### Returns

[`custom_json`](../interfaces/custom_json)

### toJSON()

> **toJSON**(`message`): `unknown`

#### Parameters

##### message

[`custom_json`](../interfaces/custom_json)

#### Returns

`unknown`
