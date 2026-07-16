[@hiveio/wax](../globals) / CxxExceptionData

# Class: CxxExceptionData

## Constructors

### new CxxExceptionData()

> **new CxxExceptionData**(`assertHash`, `code`, `message`, `name`, `stack`, `extension`): [`CxxExceptionData`](./CxxExceptionData)

#### Parameters

##### assertHash

`string`

##### code

`number`

##### message

`string`

##### name

`string`

##### stack

readonly [`IStackFrame`](../interfaces/IStackFrame)[]

##### extension

[`IExtensionData`](../interfaces/IExtensionData)

#### Returns

[`CxxExceptionData`](./CxxExceptionData)

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L30)

## Properties

### assertHash

> `readonly` **assertHash**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:31](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L31)

***

### code

> `readonly` **code**: `number`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L32)

***

### extension

> `readonly` **extension**: [`IExtensionData`](../interfaces/IExtensionData)

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L36)

***

### message

> `readonly` **message**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L33)

***

### name

> `readonly` **name**: `string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L34)

***

### stack

> `readonly` **stack**: readonly [`IStackFrame`](../interfaces/IStackFrame)[]

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L35)

## Accessors

### category

#### Get Signature

> **get** **category**(): `string`

Origin of the assertion: `"protocol"`, `"chain"`, or `"unknown"`.

##### Returns

`string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L40)

***

### extras

#### Get Signature

> **get** **extras**(): `Record`\<`string`, `any`\>

Additional fields from the top-level C++ stack frame.

##### Returns

`Record`\<`string`, `any`\>

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L68)

***

### subject

#### Get Signature

> **get** **subject**(): `unknown`

The value that failed the assertion (e.g. the invalid account name).

##### Returns

`unknown`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:63](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L63)

***

### subjectType

#### Get Signature

> **get** **subjectType**(): `string`

Kind of the value that failed validation (e.g. `"account_name"`, `"asset"`, `"balance"`).
Returns `"none"` when the top frame does not carry a subject, `"any"` when a subject is
present but no specific subject_type was recorded.

##### Returns

`string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L54)

## Methods

### formattedMessage()

> **formattedMessage**(`categoryOverride`?): `string`

#### Parameters

##### categoryOverride?

`string`

#### Returns

`string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L72)

***

### toString()

> **toString**(): `string`

#### Returns

`string`

#### Defined in

[wasm/lib/detailed/cxx\_exception\_data.ts:90](https://gitlab.syncad.com/hive/wax/-/blob/0bb90ba7370eb19c116f3d595f98326c8b50b817/ts/wasm/lib/detailed/cxx_exception_data.ts#L90)
