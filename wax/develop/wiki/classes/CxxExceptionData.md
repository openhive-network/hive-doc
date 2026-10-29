[@hiveio/wax](../globals) / CxxExceptionData

# Class: CxxExceptionData

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L29)

## Constructors

### Constructor

> **new CxxExceptionData**(`assertHash`, `code`, `message`, `name`, `stack`, `extension`): `CxxExceptionData`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L30)

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

`CxxExceptionData`

## Properties

### assertHash

> `readonly` **assertHash**: `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:31](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L31)

***

### code

> `readonly` **code**: `number`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L32)

***

### extension

> `readonly` **extension**: [`IExtensionData`](../interfaces/IExtensionData)

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L36)

***

### message

> `readonly` **message**: `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L33)

***

### name

> `readonly` **name**: `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L34)

***

### stack

> `readonly` **stack**: readonly [`IStackFrame`](../interfaces/IStackFrame)[]

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L35)

## Accessors

### category

#### Get Signature

> **get** **category**(): `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L40)

Origin of the assertion: `"protocol"`, `"chain"`, or `"unknown"`.

##### Returns

`string`

***

### extras

#### Get Signature

> **get** **extras**(): `Record`\<`string`, `any`\>

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L68)

Additional fields from the top-level C++ stack frame.

##### Returns

`Record`\<`string`, `any`\>

***

### subject

#### Get Signature

> **get** **subject**(): `unknown`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:63](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L63)

The value that failed the assertion (e.g. the invalid account name).

##### Returns

`unknown`

***

### subjectType

#### Get Signature

> **get** **subjectType**(): `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L54)

Kind of the value that failed validation (e.g. `"account_name"`, `"asset"`, `"balance"`).
Returns `"none"` when the top frame does not carry a subject, `"any"` when a subject is
present but no specific subject_type was recorded.

##### Returns

`string`

## Methods

### formattedMessage()

> **formattedMessage**(`categoryOverride?`): `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L72)

#### Parameters

##### categoryOverride?

`string`

#### Returns

`string`

***

### toString()

> **toString**(): `string`

Defined in: [wasm/lib/detailed/cxx\_exception\_data.ts:90](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/cxx_exception_data.ts#L90)

#### Returns

`string`
