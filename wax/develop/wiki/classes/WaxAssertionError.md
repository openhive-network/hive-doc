[@hiveio/wax](../globals) / WaxAssertionError

# Class: WaxAssertionError

## Extends

- [`WaxError`](./WaxError)

## Extended by

- [`WaxProtocolAssertionError`](./WaxProtocolAssertionError)
- [`WaxChainAssertionError`](./WaxChainAssertionError)

## Constructors

### new WaxAssertionError()

> **new WaxAssertionError**(`assertionHash`, `assertionData`): [`WaxAssertionError`](./WaxAssertionError)

#### Parameters

##### assertionHash

`string`

##### assertionData

`string`

#### Returns

[`WaxAssertionError`](./WaxAssertionError)

#### Overrides

[`WaxError`](./WaxError).[`constructor`](./WaxError#constructors)

#### Defined in

[wasm/lib/detailed/errors.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/errors.ts#L17)

## Properties

### assertionData

> **assertionData**: `string`

#### Defined in

[wasm/lib/detailed/errors.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/errors.ts#L15)

***

### assertionHash

> **assertionHash**: `string`

#### Defined in

[wasm/lib/detailed/errors.ts:14](https://gitlab.syncad.com/hive/wax/-/blob/c9c4918a845f59ebd97fff1316d00c91827df623/ts/wasm/lib/detailed/errors.ts#L14)

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
