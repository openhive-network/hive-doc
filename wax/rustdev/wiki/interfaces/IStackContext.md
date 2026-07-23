[@hiveio/wax](../globals) / IStackContext

# Interface: IStackContext

Parsed C++ exception data bridged from WASM. Pure data model — not an exception.

The underlying JSON payload uses snake_case; getters expose camelCase equivalents
for the derived values (category, subjectType, subject, extras). Raw snake_case
fields remain on the typed `stack` / `extension` members for direct inspection.

## Properties

### file

> **file**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L11)

***

### hostname

> **hostname**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L14)

***

### level

> **level**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L10)

***

### line

> **line**: `number`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L12)

***

### method

> **method**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L13)

***

### thread\_name

> **thread\_name**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L15)

***

### timestamp?

> `optional` **timestamp**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/21764f73ed0091d405f7e60622569bf2cfced3da/ts/wasm/lib/detailed/cxx_exception_data.ts#L16)
