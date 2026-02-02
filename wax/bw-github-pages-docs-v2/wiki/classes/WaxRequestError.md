[@hiveio/wax](../globals) / WaxRequestError

# Class: WaxRequestError\<T\>

## Extends

- [`WaxError`](./WaxError)

## Extended by

- [`WaxMalformedJsonError`](./WaxMalformedJsonError)
- [`WaxNon_2XX_3XX_ResponseCodeError`](./WaxNon_2XX_3XX_ResponseCodeError)
- [`WaxUnknownRequestError`](./WaxUnknownRequestError)
- [`WaxRequestTimeoutError`](./WaxRequestTimeoutError)
- [`WaxRequestAbortedByUser`](./WaxRequestAbortedByUser)

## Type Parameters

• **T** *extends* `object` \| `string` = `string`

## Constructors

### new WaxRequestError()

> **new WaxRequestError**\<`T`\>(`request`, `response`, `message`?, `source`?): [`WaxRequestError`](./WaxRequestError)\<`T`\>

#### Parameters

##### request

[`IRequestOptions`](../interfaces/IRequestOptions)

##### response

`Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

##### message?

`string`

##### source?

`Error`

#### Returns

[`WaxRequestError`](./WaxRequestError)\<`T`\>

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/healthchecker/errors.ts#L28)

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

### request

> `readonly` **request**: [`IRequestOptions`](../interfaces/IRequestOptions)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/healthchecker/errors.ts#L29)

***

### response

> `readonly` **response**: `Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/healthchecker/errors.ts#L30)

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
