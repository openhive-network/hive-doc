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

[src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/2f7a27aae75211cc09d0f6d9a283eb08aad0f8bb/src/interfaces.ts#L234)
