[@hiveio/wax](../globals) / WaxAssertionError

# Class: WaxAssertionError

Base class for C++ assertion errors raised by the Hive protocol or chain layer.

Subclasses cover common "what went wrong" cases (invalid account name, insufficient
balance, invalid asset, etc.). Assertions that do not match any subclass are raised
as `WaxAssertionError` itself; callers can inspect `category`, `subjectType` and
`subject` to identify the exact assertion.

## Extends

- [`WaxError`](./WaxError)

## Extended by

- [`WaxUnhandledAssertionError`](./WaxUnhandledAssertionError)
- [`WaxInvalidAccountNameError`](./WaxInvalidAccountNameError)
- [`WaxInvalidPermlinkError`](./WaxInvalidPermlinkError)
- [`WaxInvalidAssetError`](./WaxInvalidAssetError)
- [`WaxInvalidFeeError`](./WaxInvalidFeeError)
- [`WaxInsufficientBalanceError`](./WaxInsufficientBalanceError)

## Constructors

### new WaxAssertionError()

> **new WaxAssertionError**(`raw`, `category`?): [`WaxAssertionError`](./WaxAssertionError)

#### Parameters

##### raw

[`CxxExceptionData`](./CxxExceptionData)

##### category?

`string`

#### Returns

[`WaxAssertionError`](./WaxAssertionError)

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/errors.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L35)

## Properties

### cause?

> `optional` **cause**: `unknown`

#### Inherited from

[`WaxError`](./WaxError).[`cause`](./WaxError#cause)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es2022.error.d.ts:26

***

### message

> **message**: `string`

#### Inherited from

[`WaxError`](./WaxError).[`message`](./WaxError#message)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1077

***

### name

> **name**: `string`

#### Inherited from

[`WaxError`](./WaxError).[`name`](./WaxError#name)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1076

***

### raw

> `readonly` **raw**: [`CxxExceptionData`](./CxxExceptionData)

#### Defined in

[wasm/lib/detailed/errors.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L32)

***

### stack?

> `optional` **stack**: `string`

#### Inherited from

[`WaxError`](./WaxError).[`stack`](./WaxError#stack)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1078

***

### prepareStackTrace()?

> `static` `optional` **prepareStackTrace**: (`err`, `stackTraces`) => `any`

Optional override for formatting stack traces

#### Parameters

##### err

`Error`

##### stackTraces

`CallSite`[]

#### Returns

`any`

#### See

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

#### Inherited from

[`WaxError`](./WaxError).[`prepareStackTrace`](./WaxError#preparestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:143

***

### stackTraceLimit

> `static` **stackTraceLimit**: `number`

#### Inherited from

[`WaxError`](./WaxError).[`stackTraceLimit`](./WaxError#stacktracelimit)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:145

## Accessors

### assertHash

#### Get Signature

> **get** **assertHash**(): `string`

Hash identifying the specific C++ assertion site.

##### Returns

`string`

#### Defined in

[wasm/lib/detailed/errors.ts:56](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L56)

***

### category

#### Get Signature

> **get** **category**(): `string`

Origin of the assertion: `"protocol"` or `"chain"`.

##### Returns

`string`

#### Defined in

[wasm/lib/detailed/errors.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L44)

***

### extras

#### Get Signature

> **get** **extras**(): `Record`\<`string`, `any`\>

Additional fields from the top-level C++ stack frame.

##### Returns

`Record`\<`string`, `any`\>

#### Defined in

[wasm/lib/detailed/errors.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L53)

***

### subject

#### Get Signature

> **get** **subject**(): `unknown`

The value that failed the assertion.

##### Returns

`unknown`

#### Defined in

[wasm/lib/detailed/errors.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L50)

***

### subjectType

#### Get Signature

> **get** **subjectType**(): `string`

Kind of the value that failed validation (e.g. `"account_name"`, `"asset"`, `"balance"`).

##### Returns

`string`

#### Defined in

[wasm/lib/detailed/errors.ts:47](https://gitlab.syncad.com/hive/wax/-/blob/296332e5da2d278371ae5dcea3694c4c9523c8db/ts/wasm/lib/detailed/errors.ts#L47)

## Methods

### captureStackTrace()

> `static` **captureStackTrace**(`targetObject`, `constructorOpt`?): `void`

Create .stack property on a target object

#### Parameters

##### targetObject

`object`

##### constructorOpt?

`Function`

#### Returns

`void`

#### Inherited from

[`WaxError`](./WaxError).[`captureStackTrace`](./WaxError#capturestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:136
