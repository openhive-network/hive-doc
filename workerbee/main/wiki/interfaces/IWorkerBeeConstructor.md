[@hiveio/workerbee](../globals) / IWorkerBeeConstructor

# Interface: IWorkerBeeConstructor

Defined in: [src/interfaces.ts:226](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/interfaces.ts#L226)

## Constructors

### Constructor

> **new IWorkerBeeConstructor**(`chain`): [`IWorkerBee`](./IWorkerBee)

Defined in: [src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/641ebd4057420d4440d52d6ceb6edbf663489747/src/interfaces.ts#L234)

Constructs new WorkerBee bot object

#### Parameters

##### chain

`IHiveChainInterface`

Chain interface to the hive compatible chain

#### Returns

[`IWorkerBee`](./IWorkerBee)

#### Note

If you do not register an "error" event listener, the error will be dropped silently
