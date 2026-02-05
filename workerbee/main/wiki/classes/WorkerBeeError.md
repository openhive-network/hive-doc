[@hiveio/workerbee](../globals) / WorkerBeeError

# Class: WorkerBeeError

**`Internal`**

## Extends

- `Error`

## Constructors

### new WorkerBeeError()

> **new WorkerBeeError**(`message`, `originator`?): [`WorkerBeeError`](./WorkerBeeError)

#### Parameters

##### message

`string`

##### originator?

`any`

#### Returns

[`WorkerBeeError`](./WorkerBeeError)

#### Overrides

`Error.constructor`

#### Defined in

[src/errors.ts:5](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/errors.ts#L5)

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

node\_modules/.pnpm/@types+node@20.17.19/node\_modules/@types/node/globals.d.ts:98

***

### stackTraceLimit

> `static` **stackTraceLimit**: `number`

#### Inherited from

`Error.stackTraceLimit`

#### Defined in

node\_modules/.pnpm/@types+node@20.17.19/node\_modules/@types/node/globals.d.ts:100

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

node\_modules/.pnpm/@types+node@20.17.19/node\_modules/@types/node/globals.d.ts:91
