[@hiveio/wax](../globals) / WaxError

# Class: WaxError

## Extends

- `Error`

## Extended by

- [`WaxHealthCheckerError`](./WaxHealthCheckerError)
- [`WaxHealthCheckerValidatorFailedError`](./WaxHealthCheckerValidatorFailedError)
- [`WaxRequestError`](./WaxRequestError)
- [`WaxAssertionError`](./WaxAssertionError)
- [`WaxChainApiError`](./WaxChainApiError)
- [`WaxPrivateKeyLeakDetectedException`](./WaxPrivateKeyLeakDetectedException)

## Constructors

### new WaxError()

> **new WaxError**(`message`?, `source`?): [`WaxError`](./WaxError)

#### Parameters

##### message?

`string`

##### source?

`Error`

#### Returns

[`WaxError`](./WaxError)

#### Overrides

`Error.constructor`

#### Defined in

[wasm/lib/detailed/errors.ts:7](https://gitlab.syncad.com/hive/wax/-/blob/8f4868a84978a3f8c750536f945a2a0ec7470397/ts/wasm/lib/detailed/errors.ts#L7)

## Properties

### cause?

> `optional` **cause**: `unknown`

#### Inherited from

`Error.cause`

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es2022.error.d.ts:26

***

### message

> **message**: `string`

#### Inherited from

`Error.message`

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1077

***

### name

> **name**: `string`

#### Inherited from

`Error.name`

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1076

***

### stack?

> `optional` **stack**: `string`

#### Inherited from

`Error.stack`

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

`Error.prepareStackTrace`

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:143

***

### stackTraceLimit

> `static` **stackTraceLimit**: `number`

#### Inherited from

`Error.stackTraceLimit`

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

`Error.captureStackTrace`

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:136
