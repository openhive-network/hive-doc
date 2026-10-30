[@hiveio/workerbee](../globals) / IWorkerBee

# Interface: IWorkerBee

Defined in: [src/interfaces.ts:32](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L32)

## Properties

### chain

> `readonly` **chain**: `TWaxExtended`\<`WaxExtendTypes`\>

Defined in: [src/interfaces.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L43)

Exposed hive chain interface we are using.

***

### running

> `readonly` **running**: `boolean`

Defined in: [src/interfaces.ts:38](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L38)

Indicates if the bot is running

## Accessors

### observe

#### Get Signature

> **get** **observe**(): `QueenBee`

Defined in: [src/interfaces.ts:132](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L132)

Allows you to iterate over blocks in live mode

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Example

```ts
workerbee.observe.onBlock().subscribe({
  next: (data) => {
    console.log(data);
  },
  error: console.error
});
```

##### Returns

`QueenBee`

## Methods

### \[asyncIterator\]()

> **\[asyncIterator\]**(): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

Defined in: [src/interfaces.ts:168](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L168)

Allows you to iterate over blocks indefinitely

Ignores errors

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

#### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

#### Example

```ts
for await (const block of workerbee) {
  console.log(block);
}
```

***

### broadcast()

> **broadcast**(`tx`, `options?`): `Promise`\<`void`\>

Defined in: [src/interfaces.ts:152](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L152)

Broadcast given transaction to the remote and returns a promise resolved when
transaction has been successfully applied on chain.
You can also optionally provide [verifySignatures](./IBroadcastOptions) option
if you want to ensure that the signatures in the transaction, applied on chain match the local ones.

Requires signed transaction

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

#### Parameters

##### tx

`ApiTransaction` \| `ITransaction`

Protobuf transactoin to broadcast

##### options?

[`IBroadcastOptions`](./IBroadcastOptions)

Options for broadcasting

#### Returns

`Promise`\<`void`\>

***

### delete()

> **delete**(): `void`

Defined in: [src/interfaces.ts:59](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L59)

Deletes the current bot instance and underlying wax and beekepeer objects.
wax chain object is deleted only when its instance was managed by workerbee itself.

#### Returns

`void`

***

### getVersion()

> **getVersion**(): `string`

Defined in: [src/interfaces.ts:137](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L137)

#### Returns

`string`

The version of the library

***

### iterate()

#### Call Signature

> **iterate**(): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

Defined in: [src/interfaces.ts:184](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L184)

Allows you to iterate over blocks indefinitely - alias to async iterator

Ignores errors

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

##### Example

```ts
for await (const block of workerbee.iterate()) {
  console.log(block);
}
```

#### Call Signature

> **iterate**(`throwOnError`): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

Defined in: [src/interfaces.ts:206](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L206)

Allows you to iterate over blocks indefinitely - alias to async iterator

Allows to handle errors via try/catch clause around the async iterator

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### throwOnError

`boolean`

If true, the error will be thrown

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

##### Example

```ts
try {
  for await (const block of workerbee.iterate(true)) {
    console.log(block);
  }
} catch (error) {
  console.error("Error while iterating:", error);
}
```

#### Call Signature

> **iterate**(`errorHandler`): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

Defined in: [src/interfaces.ts:223](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L223)

Allows you to iterate over blocks indefinitely - alias to async iterator

Allows to handle errors via callback

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### errorHandler

(`error`) => `void`

Callback function to handle errors

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData)\>

##### Example

```ts
for await (const block of workerbee.iterate(console.error))
  console.log(block);
```

***

### providePastOperations()

#### Call Signature

> **providePastOperations**(`fromBlock`, `toBlock`): `TPastQueen`

Defined in: [src/interfaces.ts:86](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L86)

Allows you to iterate over blocks in the past from a given range

Note: This should be called only once per instance.
If you want to iterate over multiple ranges, you should create a new instance of WorkerBee.

Data collected by this method will be preserved for later usage by the live observer.

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### fromBlock

`number`

###### toBlock

`number`

##### Returns

`TPastQueen`

##### Example

```ts
await new Promise((resolve, reject) => {
  workerbee.providePastOperations(10_000, 10_500).onBlock().subscribe({
    next: (data) => {
      console.log(data);
    },
    error: reject,
    complete: resolve
  });
});
```

##### Throws

if called before [start](./#start)

#### Call Signature

> **providePastOperations**(`relativeTime`): `Promise`\<`TPastQueen`\>

Defined in: [src/interfaces.ts:115](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L115)

Allows you to iterate over blocks in the past from a given range

Note: This should be called only once per instance.
If you want to iterate over multiple ranges, you should create a new instance of WorkerBee.

Data collected by this method will be preserved for later usage by the live observer.

Note: Call [start](./#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### relativeTime

`string`

##### Returns

`Promise`\<`TPastQueen`\>

##### Example

```ts
workerbee.providePastOperations('-7d').then((provider) => {
  provider.onBlock().subscribe({
    next: (data) => {
      console.log(data);
    },
    error: console.error,
    complete: () => {
     console.log('Completed');
    }
  });
});
```

##### Throws

if called before [start](./#start)

***

### start()

> **start**(): `void`

Defined in: [src/interfaces.ts:48](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L48)

Starts the automation with given configuration

#### Returns

`void`

***

### stop()

> **stop**(): `void`

Defined in: [src/interfaces.ts:53](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L53)

Request automation stop

#### Returns

`void`
