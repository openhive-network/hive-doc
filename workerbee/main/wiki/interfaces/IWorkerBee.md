[@hiveio/workerbee](../globals) / IWorkerBee

# Interface: IWorkerBee

## Properties

### chain

> `readonly` **chain**: `TWaxExtended`\<`WaxExtendTypes`\>

Exposed hive chain interface we are using.

#### Defined in

[src/interfaces.ts:43](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L43)

***

### running

> `readonly` **running**: `boolean`

Indicates if the bot is running

#### Defined in

[src/interfaces.ts:38](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L38)

## Accessors

### observe

#### Get Signature

> **get** **observe**(): `QueenBee`\<`object`\>

Allows you to iterate over blocks in live mode

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

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

`QueenBee`\<`object`\>

#### Defined in

[src/interfaces.ts:132](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L132)

## Methods

### \[asyncIterator\]()

> **\[asyncIterator\]**(): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

Allows you to iterate over blocks indefinitely

Ignores errors

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

#### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

#### Example

```ts
for await (const block of workerbee) {
  console.log(block);
}
```

#### Defined in

[src/interfaces.ts:168](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L168)

***

### broadcast()

> **broadcast**(`tx`, `options`?): `Promise`\<`void`\>

Broadcast given transaction to the remote and returns a promise resolved when
transaction has been successfully applied on chain.
You can also optionally provide [verifySignatures](./IBroadcastOptions) option
if you want to ensure that the signatures in the transaction, applied on chain match the local ones.

Requires signed transaction

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

#### Parameters

##### tx

Protobuf transactoin to broadcast

`ApiTransaction` | `ITransaction`

##### options?

[`IBroadcastOptions`](./IBroadcastOptions)

Options for broadcasting

#### Returns

`Promise`\<`void`\>

#### Defined in

[src/interfaces.ts:152](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L152)

***

### delete()

> **delete**(): `void`

Deletes the current bot instance and underlying wax and beekepeer objects.
wax chain object is deleted only when its instance was managed by workerbee itself.

#### Returns

`void`

#### Defined in

[src/interfaces.ts:59](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L59)

***

### getVersion()

> **getVersion**(): `string`

#### Returns

`string`

The version of the library

#### Defined in

[src/interfaces.ts:137](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L137)

***

### iterate()

#### Call Signature

> **iterate**(): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

Allows you to iterate over blocks indefinitely - alias to async iterator

Ignores errors

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

##### Example

```ts
for await (const block of workerbee.iterate()) {
  console.log(block);
}
```

##### Defined in

[src/interfaces.ts:184](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L184)

#### Call Signature

> **iterate**(`throwOnError`): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

Allows you to iterate over blocks indefinitely - alias to async iterator

Allows to handle errors via try/catch clause around the async iterator

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### throwOnError

`boolean`

If true, the error will be thrown

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

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

##### Defined in

[src/interfaces.ts:206](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L206)

#### Call Signature

> **iterate**(`errorHandler`): `AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

Allows you to iterate over blocks indefinitely - alias to async iterator

Allows to handle errors via callback

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

##### Parameters

###### errorHandler

(`error`) => `void`

Callback function to handle errors

##### Returns

`AsyncIterator`\<[`IBlockData`](./IBlockData) & [`IBlockHeaderData`](./IBlockHeaderData), `any`, `any`\>

##### Example

```ts
for await (const block of workerbee.iterate(console.error))
  console.log(block);
```

##### Defined in

[src/interfaces.ts:223](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L223)

***

### providePastOperations()

#### Call Signature

> **providePastOperations**(`fromBlock`, `toBlock`): `TPastQueen`

Allows you to iterate over blocks in the past from a given range

Note: This should be called only once per instance.
If you want to iterate over multiple ranges, you should create a new instance of WorkerBee.

Data collected by this method will be preserved for later usage by the live observer.

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

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

if called before [start](./IWorkerBee#start)

##### Defined in

[src/interfaces.ts:86](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L86)

#### Call Signature

> **providePastOperations**(`relativeTime`): `Promise`\<`TPastQueen`\>

Allows you to iterate over blocks in the past from a given range

Note: This should be called only once per instance.
If you want to iterate over multiple ranges, you should create a new instance of WorkerBee.

Data collected by this method will be preserved for later usage by the live observer.

Note: Call [start](./IWorkerBee#start) explicitly by yourself if the bot is not running yet, either before this or directly after.

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

if called before [start](./IWorkerBee#start)

##### Defined in

[src/interfaces.ts:115](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L115)

***

### start()

> **start**(): `void`

Starts the automation with given configuration

#### Returns

`void`

#### Defined in

[src/interfaces.ts:48](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L48)

***

### stop()

> **stop**(): `void`

Request automation stop

#### Returns

`void`

#### Defined in

[src/interfaces.ts:53](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/interfaces.ts#L53)
