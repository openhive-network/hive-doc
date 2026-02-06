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

[src/interfaces.ts:234](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/interfaces.ts#L234)
