# EquipmentSlot

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.entity.equipment.EquipmentSlot;
```


## Enum Constants

EquipmentSlot is an enum. It has 6 enum constants. They are accessible using the code below.

```zenscript
<constant:minecraft:equipmentslot:mainhand>
<constant:minecraft:equipmentslot:offhand>
<constant:minecraft:equipmentslot:feet>
<constant:minecraft:equipmentslot:legs>
<constant:minecraft:equipmentslot:chest>
<constant:minecraft:equipmentslot:head>
```
## Methods

:::group{name=getCommandString}

Return Type: string

```zenscript
// EquipmentSlot.getCommandString() as string

myEquipmentSlot.getCommandString();
```

:::

:::group{name=getIndex}

Return Type: int

```zenscript
// EquipmentSlot.getIndex() as int

myEquipmentSlot.getIndex();
```

:::

:::group{name=getName}

Return Type: string

```zenscript
// EquipmentSlot.getName() as string

myEquipmentSlot.getName();
```

:::

:::group{name=getType}

Return Type: [EquipmentSlotType](/vanilla/api/entity/equipment/EquipmentSlotType)

```zenscript
// EquipmentSlot.getType() as EquipmentSlotType

myEquipmentSlot.getType();
```

:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| commandString | string | true | false | No Description Provided |
| index | int | true | false | No Description Provided |
| name | string | true | false | No Description Provided |
| type | [EquipmentSlotType](/vanilla/api/entity/equipment/EquipmentSlotType) | true | false | No Description Provided |

