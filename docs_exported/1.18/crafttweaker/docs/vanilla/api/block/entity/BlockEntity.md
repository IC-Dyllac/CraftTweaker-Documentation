# BlockEntity

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.block.entity.BlockEntity;
```


## Methods

:::group{name=getBlockPos}

Return Type: [BlockPos](/vanilla/api/util/math/BlockPos)

```zenscript
// BlockEntity.getBlockPos() as BlockPos

myBlockEntity.getBlockPos();
```

:::

:::group{name=getBlockState}

Return Type: [BlockState](/vanilla/api/block/BlockState)

```zenscript
// BlockEntity.getBlockState() as BlockState

myBlockEntity.getBlockState();
```

:::

:::group{name=getLevel}

Return Type: [Level](/vanilla/api/world/Level)

```zenscript
// BlockEntity.getLevel() as Level

myBlockEntity.getLevel();
```

:::

:::group{name=hasLevel}

Return Type: boolean

```zenscript
// BlockEntity.hasLevel() as boolean

myBlockEntity.hasLevel();
```

:::

:::group{name=setData}

Return Type: void

```zenscript
BlockEntity.setData(data as MapData) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| data | [MapData](/vanilla/api/data/MapData) | No Description Provided |


:::

:::group{name=updateData}

Return Type: void

```zenscript
BlockEntity.updateData(data as MapData) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| data | [MapData](/vanilla/api/data/MapData) | No Description Provided |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| blockPos | [BlockPos](/vanilla/api/util/math/BlockPos) | true | false | No Description Provided |
| blockState | [BlockState](/vanilla/api/block/BlockState) | true | false | No Description Provided |
| data | [MapData](/vanilla/api/data/MapData) | true | true | No Description Provided |
| hasLevel | boolean | true | false | No Description Provided |
| level | [Level](/vanilla/api/world/Level) | true | false | No Description Provided |

