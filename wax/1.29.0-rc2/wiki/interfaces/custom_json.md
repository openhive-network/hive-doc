[@hiveio/wax](../globals) / custom\_json

# Interface: custom\_json

The operation custom_json_operation works similar as custom_operation,
but it is designed to be human readable/developer friendly.
The custom_json_operation is larger than custom_operation or custom_binary, that is why it costs more RC.
It should be signed as required in { required_auths } or { required_posting_auths }.
The examples of custom_json_operation:
- reblog
- muted
- pinned
- follow

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/18_custom_json.md?ref_type=heads

## Properties

### id

> **id**: `string`

#### Param

Must be less than 32 characters long.

#### Defined in

wasm/lib/proto/custom\_json.ts:24

***

### json

> **json**: `string`

#### Param

Must be a proper utf8 JSON string.

#### Defined in

wasm/lib/proto/custom\_json.ts:26

***

### required\_auths

> **required\_auths**: `string`[]

#### Param

#### Defined in

wasm/lib/proto/custom\_json.ts:20

***

### required\_posting\_auths

> **required\_posting\_auths**: `string`[]

#### Param

#### Defined in

wasm/lib/proto/custom\_json.ts:22
