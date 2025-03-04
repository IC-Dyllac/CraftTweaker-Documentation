# AbstractVillager

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.entity.type.villager.AbstractVillager;
```


## Implemented Interfaces
AbstractVillager implements the following interfaces. That means all methods defined in these interfaces are also available in AbstractVillager

- [Merchant](/vanilla/api/entity/type/villager/Merchant)

## Methods

:::group{name=getUnhappyCounter}

Return Type: int

```zenscript
// AbstractVillager.getUnhappyCounter() as int

myAbstractVillager.getUnhappyCounter();
```

:::

:::group{name=isTrading}

Return Type: boolean

```zenscript
// AbstractVillager.isTrading() as boolean

myAbstractVillager.isTrading();
```

:::

:::group{name=playCelebrateSound}

Return Type: void

```zenscript
// AbstractVillager.playCelebrateSound() as void

myAbstractVillager.playCelebrateSound();
```

:::

:::group{name=setUnhappyCounter}

Return Type: void

```zenscript
AbstractVillager.setUnhappyCounter(unhappyCounter as int) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| unhappyCounter | int | No Description Provided |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| isTrading | boolean | true | false | No Description Provided |
| unhappyCounter | int | true | true | No Description Provided |

