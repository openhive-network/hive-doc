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

[src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/b90beefe2138db7c7c82f316cc8e8ea954f21c30/src/interfaces.ts#L234)
