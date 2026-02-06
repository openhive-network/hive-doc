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

[src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/5a4fea5cf91e40d3722f05ff430c20a9f5a0ca12/src/interfaces.ts#L234)
