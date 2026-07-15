[@hiveio/wax](../globals) / WaxInvalidAssetError

# Class: WaxInvalidAssetError

Raised when an asset is invalid (wrong type, zero/negative amount, bad precision, etc.).

## Extends

- [`WaxAssertionError`](./WaxAssertionError)

## Constructors

### new WaxInvalidAssetError()

> **new WaxInvalidAssetError**(`raw`, `category`?): [`WaxInvalidAssetError`](./WaxInvalidAssetError)

#### Parameters

##### raw

[`CxxExceptionData`](./CxxExceptionData)

##### category?

`string`

#### Returns

[`WaxInvalidAssetError`](./WaxInvalidAssetError)

#### Overrides

[`WaxAssertionError`](./WaxAssertionError).[`constructor`](./WaxAssertionError#constructors)

#### Defined in

[wasm/lib/detailed/errors.ts:95](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L95)

## Properties

### cause?

> `optional` **cause**: `unknown`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`cause`](./WaxAssertionError#cause)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es2022.error.d.ts:26

***

### message

> **message**: `string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`message`](./WaxAssertionError#message)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1077

***

### name

> **name**: `string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`name`](./WaxAssertionError#name)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1076

***

### raw

> `readonly` **raw**: [`CxxExceptionData`](./CxxExceptionData)

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`raw`](./WaxAssertionError#raw)

#### Defined in

[wasm/lib/detailed/errors.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L32)

***

### stack?

> `optional` **stack**: `string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`stack`](./WaxAssertionError#stack)

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

[`WaxAssertionError`](./WaxAssertionError).[`prepareStackTrace`](./WaxAssertionError#preparestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:143

***

### stackTraceLimit

> `static` **stackTraceLimit**: `number`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`stackTraceLimit`](./WaxAssertionError#stacktracelimit)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:145

## Accessors

### assertHash

#### Get Signature

> **get** **assertHash**(): `string`

Hash identifying the specific C++ assertion site.

##### Returns

`string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`assertHash`](./WaxAssertionError#asserthash)

#### Defined in

[wasm/lib/detailed/errors.ts:56](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L56)

***

### asset

#### Get Signature

> **get** **asset**(): `unknown`

The invalid asset value, if available from the assertion data.

##### Returns

`unknown`

#### Defined in

[wasm/lib/detailed/errors.ts:101](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L101)

***

### category

#### Get Signature

> **get** **category**(): `string`

Origin of the assertion: `"protocol"` or `"chain"`.

##### Returns

`string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`category`](./WaxAssertionError#category)

#### Defined in

[wasm/lib/detailed/errors.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L44)

***

### extras

#### Get Signature

> **get** **extras**(): `Record`\<`string`, `any`\>

Additional fields from the top-level C++ stack frame.

##### Returns

`Record`\<`string`, `any`\>

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`extras`](./WaxAssertionError#extras)

#### Defined in

[wasm/lib/detailed/errors.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L53)

***

### subject

#### Get Signature

> **get** **subject**(): `unknown`

The value that failed the assertion.

##### Returns

`unknown`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`subject`](./WaxAssertionError#subject)

#### Defined in

[wasm/lib/detailed/errors.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L50)

***

### subjectType

#### Get Signature

> **get** **subjectType**(): `string`

Kind of the value that failed validation (e.g. `"account_name"`, `"asset"`, `"balance"`).

##### Returns

`string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`subjectType`](./WaxAssertionError#subjecttype)

#### Defined in

[wasm/lib/detailed/errors.ts:47](https://gitlab.syncad.com/hive/wax/-/blob/e341599adb30b8f2db12a8951f693d88322fa63b/ts/wasm/lib/detailed/errors.ts#L47)

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

[`WaxAssertionError`](./WaxAssertionError).[`captureStackTrace`](./WaxAssertionError#capturestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:136
