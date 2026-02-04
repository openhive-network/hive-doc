[@hiveio/workerbee](../globals) / IWorkerBeeConstructor

# Interface: IWorkerBeeConstructor

## Constructors

### new IWorkerBeeConstructor()

> **new IWorkerBeeConstructor**(`chain`): [`IWorkerBee`](./IWorkerBee)

Constructs new WorkerBee bot object

#### Parameters

##### chain

`IHiveChainInterface`

Chain interface to the hive compatible chain

#### Returns

[`IWorkerBee`](./IWorkerBee)

#### Note

If you do not register an "error" event listener, the error will be dropped silently

#### Defined in

[src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/b2ef1619bb44c83140e212324c99b788670cee40/src/interfaces.ts#L234)
