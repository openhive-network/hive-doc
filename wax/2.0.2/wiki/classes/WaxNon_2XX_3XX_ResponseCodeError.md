[@hiveio/wax](../globals) / WaxNon\_2XX\_3XX\_ResponseCodeError

# Class: WaxNon\_2XX\_3XX\_ResponseCodeError\<T\>

## Extends

- [`WaxRequestError`](./WaxRequestError)\<`T`\>

## Type Parameters

• **T** *extends* `object` \| `string` = `string`

## Constructors

### new WaxNon\_2XX\_3XX\_ResponseCodeError()

> **new WaxNon\_2XX\_3XX\_ResponseCodeError**\<`T`\>(`request`, `response`): [`WaxNon_2XX_3XX_ResponseCodeError`](./WaxNon_2XX_3XX_ResponseCodeError)\<`T`\>

#### Parameters

##### request

[`IRequestOptions`](../interfaces/IRequestOptions)

##### response

`Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

#### Returns

[`WaxNon_2XX_3XX_ResponseCodeError`](./WaxNon_2XX_3XX_ResponseCodeError)\<`T`\>

#### Overrides

[`WaxRequestError`](./WaxRequestError).[`constructor`](./WaxRequestError#constructors)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/healthchecker/errors.ts#L45)

## Properties

### cause?

> `optional` **cause**: `unknown`

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`cause`](./WaxRequestError#cause)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es2022.error.d.ts:26

***

### message

> **message**: `string`

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`message`](./WaxRequestError#message)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1077

***

### name

> **name**: `string`

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`name`](./WaxRequestError#name)

#### Defined in

node\_modules/.pnpm/typescript@5.7.3/node\_modules/typescript/lib/lib.es5.d.ts:1076

***

### request

> `readonly` **request**: [`IRequestOptions`](../interfaces/IRequestOptions)

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`request`](./WaxRequestError#request)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/healthchecker/errors.ts#L29)

***

### response

> `readonly` **response**: `Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`T`\>\>

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`response`](./WaxRequestError#response)

#### Defined in

[wasm/lib/detailed/healthchecker/errors.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/healthchecker/errors.ts#L30)

***

### stack?

> `optional` **stack**: `string`

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`stack`](./WaxRequestError#stack)

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

[`WaxRequestError`](./WaxRequestError).[`prepareStackTrace`](./WaxRequestError#preparestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:143

***

### stackTraceLimit

> `static` **stackTraceLimit**: `number`

#### Inherited from

[`WaxRequestError`](./WaxRequestError).[`stackTraceLimit`](./WaxRequestError#stacktracelimit)

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

[`WaxRequestError`](./WaxRequestError).[`captureStackTrace`](./WaxRequestError#capturestacktrace)

#### Defined in

node\_modules/.pnpm/@types+node@22.10.7/node\_modules/@types/node/globals.d.ts:136
