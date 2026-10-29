[@hiveio/wax](../globals) / convert

# Variable: convert

> **convert**: `object`

Defined in: wasm/lib/proto/convert.ts:12

## Type Declaration

### create()

> **create**\<`I`\>(`base?`): [`convert`](../interfaces/convert)

#### Type Parameters

##### I

`I` *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### base?

`I`

#### Returns

[`convert`](../interfaces/convert)

### fromJSON()

> **fromJSON**(`object`): [`convert`](../interfaces/convert)

#### Parameters

##### object

`any`

#### Returns

[`convert`](../interfaces/convert)

### fromPartial()

> **fromPartial**\<`I`\>(`object`): [`convert`](../interfaces/convert)

#### Type Parameters

##### I

`I` *extends* `object` & `object` & \{ \[K in string \| number \| symbol\]: never \}

#### Parameters

##### object

`I`

#### Returns

[`convert`](../interfaces/convert)

### toJSON()

> **toJSON**(`message`): `unknown`

#### Parameters

##### message

[`convert`](../interfaces/convert)

#### Returns

`unknown`
