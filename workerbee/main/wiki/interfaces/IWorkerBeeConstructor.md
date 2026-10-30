[@hiveio/workerbee](../globals) / IWorkerBeeConstructor

# Interface: IWorkerBeeConstructor

Defined in: [src/interfaces.ts:226](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L226)

## Constructors

### Constructor

> **new IWorkerBeeConstructor**(`chain`): [`IWorkerBee`](./IWorkerBee)

Defined in: [src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/interfaces.ts#L234)

Constructs new WorkerBee bot object

#### Parameters

##### chain

`IHiveChainInterface`

Chain interface to the hive compatible chain

#### Returns

[`IWorkerBee`](./IWorkerBee)

#### Note

If you do not register an "error" event listener, the error will be dropped silently
