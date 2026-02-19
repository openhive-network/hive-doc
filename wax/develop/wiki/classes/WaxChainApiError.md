[@hiveio/wax](../globals) / WaxChainApiError

# Class: WaxChainApiError

## Extends

- [`WaxError`](./WaxError)

## Constructors

### new WaxChainApiError()

> **new WaxChainApiError**(`message`, `request`, `response`, `cause`?): [`WaxChainApiError`](./WaxChainApiError)

#### Parameters

##### message

`string`

##### request

`TInterceptorRequestOptions`

##### response

`Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`any`\>\>

##### cause?

`Error`

#### Returns

[`WaxChainApiError`](./WaxChainApiError)

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/errors.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/ac0ea25b3e26f059ca8c3033877d3dc56983d37a/ts/wasm/lib/detailed/errors.ts#L40)

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

> `readonly` **request**: `TInterceptorRequestOptions`

#### Defined in

[wasm/lib/detailed/errors.ts:42](https://gitlab.syncad.com/hive/wax/-/blob/ac0ea25b3e26f059ca8c3033877d3dc56983d37a/ts/wasm/lib/detailed/errors.ts#L42)

***

### response

> `readonly` **response**: `Partial`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`any`\>\>

#### Defined in

[wasm/lib/detailed/errors.ts:43](https://gitlab.syncad.com/hive/wax/-/blob/ac0ea25b3e26f059ca8c3033877d3dc56983d37a/ts/wasm/lib/detailed/errors.ts#L43)

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
