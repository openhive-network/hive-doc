[@hiveio/wax](../globals) / WaxHealthCheckerError

# Class: WaxHealthCheckerError

## Extends

- [`WaxError`](./WaxError)

## Constructors

### new WaxHealthCheckerError()

> **new WaxHealthCheckerError**(`cause`, `apiEndpoint`, `apiUrl`?): [`WaxHealthCheckerError`](./WaxHealthCheckerError)

#### Parameters

##### cause

`Error`

##### apiEndpoint

[`IHiveEndpoint`](../interfaces/IHiveEndpoint)

##### apiUrl?

`string`

#### Returns

[`WaxHealthCheckerError`](./WaxHealthCheckerError)

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:6](https://gitlab.syncad.com/hive/wax/-/blob/25b077f1212af270804d5f80de54dc9af4e3c0b0/ts/wasm/lib/detailed/healthchecker/errors.ts#L6)

## Properties

### apiEndpoint

> `readonly` **apiEndpoint**: [`IHiveEndpoint`](../interfaces/IHiveEndpoint)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/25b077f1212af270804d5f80de54dc9af4e3c0b0/ts/wasm/lib/detailed/healthchecker/errors.ts#L8)

***

### apiUrl?

> `readonly` `optional` **apiUrl**: `string`

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/25b077f1212af270804d5f80de54dc9af4e3c0b0/ts/wasm/lib/detailed/healthchecker/errors.ts#L9)

***

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
