[@hiveio/wax](../globals) / WaxHealthCheckerValidatorFailedError

# Class: WaxHealthCheckerValidatorFailedError\<T\>

## Extends

- [`WaxError`](./WaxError)

## Type Parameters

• **T** *extends* `object` \| `string` = `string`

## Constructors

### new WaxHealthCheckerValidatorFailedError()

> **new WaxHealthCheckerValidatorFailedError**\<`T`\>(`failedReason`, `apiEndpoint`, `request`, `response`): [`WaxHealthCheckerValidatorFailedError`](./WaxHealthCheckerValidatorFailedError)\<`T`\>

#### Parameters

##### failedReason

`string`

##### apiEndpoint

[`IHiveEndpoint`](../interfaces/IHiveEndpoint)

##### request

[`IRequestOptions`](../interfaces/IRequestOptions)

##### response

`Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

#### Returns

[`WaxHealthCheckerValidatorFailedError`](./WaxHealthCheckerValidatorFailedError)\<`T`\>

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/healthchecker/errors.ts#L16)

## Properties

### apiEndpoint

> `readonly` **apiEndpoint**: [`IHiveEndpoint`](../interfaces/IHiveEndpoint)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/healthchecker/errors.ts#L18)

***

### cause?

> `optional` **cause**: `unknown`

#### Inherited from

[`WaxError`](./WaxError).[`cause`](./WaxError#cause)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es2022.error.d.ts:26

***

### failedReason

> `readonly` **failedReason**: `string`

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/healthchecker/errors.ts#L17)

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

### request

> `readonly` **request**: [`IRequestOptions`](../interfaces/IRequestOptions)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:19](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/healthchecker/errors.ts#L19)

***

### response

> `readonly` **response**: `Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/healthchecker/errors.ts#L20)

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
