[@hiveio/workerbee](../globals) / IWorkerBeeConstructor

# Interface: IWorkerBeeConstructor

Defined in: [src/interfaces.ts:226](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/interfaces.ts#L226)

## Constructors

### Constructor

> **new IWorkerBeeConstructor**(`chain`): [`IWorkerBee`](./IWorkerBee)

Defined in: [src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/interfaces.ts#L234)

Constructs new WorkerBee bot object

#### Parameters

##### chain

`IHiveChainInterface`

Chain interface to the hive compatible chain

#### Returns

[`IWorkerBee`](./IWorkerBee)

#### Note

If you do not register an "error" event listener, the error will be dropped silently
