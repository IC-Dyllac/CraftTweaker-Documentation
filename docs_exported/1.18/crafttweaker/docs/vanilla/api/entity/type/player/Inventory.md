# Inventory

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.entity.type.player.Inventory;
```


## Implemented Interfaces
Inventory implements the following interfaces. That means all methods defined in these interfaces are also available in Inventory

- [Container](/vanilla/api/world/Container)
- [Nameable](/vanilla/api/world/Nameable)

## Methods

:::group{name=add}

Return Type: boolean

```zenscript
Inventory.add(stack as ItemStack) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=add}

Return Type: boolean

```zenscript
Inventory.add(index as int, stack as ItemStack) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| index | int | No Description Provided |
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=contains}

Return Type: boolean

```zenscript
Inventory.contains(stack as ItemStack) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=contains}

Return Type: boolean

```zenscript
Inventory.contains(tag as KnownTag<ItemDefinition>) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| tag | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;[ItemDefinition](/vanilla/api/item/ItemDefinition)&gt; | No Description Provided |


:::

:::group{name=dropAll}

Return Type: void

```zenscript
// Inventory.dropAll() as void

myInventory.dropAll();
```

:::

:::group{name=findSlotMatchingItem}

Return Type: int

```zenscript
Inventory.findSlotMatchingItem(stack as ItemStack) as int
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=findSlotMatchingUnusedItem}

Return Type: int

```zenscript
Inventory.findSlotMatchingUnusedItem(stack as ItemStack) as int
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=getArmor}

Return Type: [ItemStack](/vanilla/api/item/ItemStack)

```zenscript
Inventory.getArmor(armorIndex as int) as ItemStack
```

| Parameter | Type | Description |
|-----------|------|-------------|
| armorIndex | int | No Description Provided |


:::

:::group{name=getFreeSlot}

Return Type: int

```zenscript
// Inventory.getFreeSlot() as int

myInventory.getFreeSlot();
```

:::

:::group{name=getSelected}

Return Type: [ItemStack](/vanilla/api/item/ItemStack)

```zenscript
// Inventory.getSelected() as ItemStack

myInventory.getSelected();
```

:::

:::group{name=getSlotWithRemainingSpace}

Return Type: int

```zenscript
Inventory.getSlotWithRemainingSpace(stack as ItemStack) as int
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=getSuitableHotbarSlot}

Return Type: int

```zenscript
// Inventory.getSuitableHotbarSlot() as int

myInventory.getSuitableHotbarSlot();
```

:::

:::group{name=getTimesChanged}

Return Type: int

```zenscript
// Inventory.getTimesChanged() as int

myInventory.getTimesChanged();
```

:::

:::group{name=hurtArmor}

Return Type: void

```zenscript
Inventory.hurtArmor(source as DamageSource, damage as float, armorSlots as int[]) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| source | [DamageSource](/vanilla/api/world/DamageSource) | No Description Provided |
| damage | float | No Description Provided |
| armorSlots | int[] | No Description Provided |


:::

:::group{name=pickSlot}

Return Type: void

```zenscript
Inventory.pickSlot(index as int) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| index | int | No Description Provided |


:::

:::group{name=removeItem}

Return Type: void

```zenscript
Inventory.removeItem(stack as ItemStack) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::

:::group{name=setPickedItem}

Return Type: void

```zenscript
Inventory.setPickedItem(stack as ItemStack) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [ItemStack](/vanilla/api/item/ItemStack) | No Description Provided |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| freeSlot | int | true | false | No Description Provided |
| selected | [ItemStack](/vanilla/api/item/ItemStack) | true | false | No Description Provided |
| suitableHotbarSlot | int | true | false | No Description Provided |
| timesChanged | int | true | false | No Description Provided |

