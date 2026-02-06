[@hiveio/wax](../globals) / WaxProtocolAssertionError

# Class: WaxProtocolAssertionError

## Extends

- [`WaxAssertionError`](./WaxAssertionError)

## Constructors

### new WaxProtocolAssertionError()

> **new WaxProtocolAssertionError**(`assertionHash`, `assertionData`): [`WaxProtocolAssertionError`](./WaxProtocolAssertionError)

#### Parameters

##### assertionHash

`string`

##### assertionData

`string`

#### Returns

[`WaxProtocolAssertionError`](./WaxProtocolAssertionError)

#### Overrides

[`WaxAssertionError`](./WaxAssertionError).[`constructor`](./WaxAssertionError#constructors)

#### Defined in

[wasm/lib/detailed/errors.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/99f67a8c04ccce81c4687346434ed0802c9d7d6a/ts/wasm/lib/detailed/errors.ts#L26)

## Properties

### assertionData

> **assertionData**: `string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`assertionData`](./WaxAssertionError#assertiondata)

#### Defined in

[wasm/lib/detailed/errors.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/99f67a8c04ccce81c4687346434ed0802c9d7d6a/ts/wasm/lib/detailed/errors.ts#L15)

***

### assertionHash

> **assertionHash**: `string`

#### Inherited from

[`WaxAssertionError`](./WaxAssertionError).[`assertionHash`](./WaxAssertionError#assertionhash)

#### Defined in

[wasm/lib/detailed/errors.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/99f67a8c04ccce81c4687346434ed0802c9d7d6a/ts/wasm/lib/detailed/errors.ts#L14)

***

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
