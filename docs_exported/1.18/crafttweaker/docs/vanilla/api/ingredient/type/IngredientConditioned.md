# IngredientConditioned&LT;T : IIngredient&GT;

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.ingredient.type.IngredientConditioned;
```


## Implemented Interfaces
IngredientConditioned implements the following interfaces. That means all methods defined in these interfaces are also available in IngredientConditioned

- [IIngredient](/vanilla/api/ingredient/IIngredient)

## Casters

| Result type | Is Implicit |
|-------------|-------------|
| [IData](/vanilla/api/data/IData) | true |
| [IIngredientWithAmount](/vanilla/api/ingredient/IIngredientWithAmount) | true |
| [MapData](/vanilla/api/data/MapData) | true |

## Methods

:::group{name=addGlobalAttributeModifier}

Adds an AttributeModifier to this IIngredient.

 Attributes added with this method appear on all ItemStacks that match this IIngredient,
 regardless of how or when the ItemStack was made, if you want to have the attribute on a
 single specific ItemStack (such as a specific Diamond Sword made in a recipe), then you should use
 IItemStack#withAttributeModifier

Return Type: void

```zenscript
// IngredientConditioned.addGlobalAttributeModifier(attribute as Attribute, name as string, value as double, operation as AttributeOperation, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.addGlobalAttributeModifier(<attribute:minecraft:generic.attack_damage>, "Extra Power", 10, AttributeOperation.ADDITION, [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| attribute | [Attribute](/vanilla/api/entity/attribute/Attribute) | The Attribute of the modifier. |
| name | string | The name of the modifier. |
| value | double | The value of the modifier. |
| operation | [AttributeOperation](/vanilla/api/entity/attribute/AttributeOperation) | The operation of the modifier. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | What slots the modifier is valid for. |


:::

:::group{name=addGlobalAttributeModifier}

Adds an AttributeModifier to this IIngredient using a specific UUID.

 The UUID can be used to override an existing attribute on an ItemStack with this new modifier.
 You can use `/ct hand attributes` to get the UUID of the attributes on an ItemStack.

 Attributes added with this method appear on all ItemStacks that match this IIngredient,
 regardless of how or when the ItemStack was made, if you want to have the attribute on a
 single specific ItemStack (such as a specific Diamond Sword made in a recipe), then you should use
 IItemStack#withAttributeModifier

Return Type: void

```zenscript
// IngredientConditioned.addGlobalAttributeModifier(attribute as Attribute, uuid as invalid, name as string, value as double, operation as AttributeOperation, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.addGlobalAttributeModifier(<attribute:minecraft:generic.attack_damage>, IItemStack.BASE_ATTACK_DAMAGE_UUID, "Extra Power", 10, AttributeOperation.ADDITION, [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| attribute | [Attribute](/vanilla/api/entity/attribute/Attribute) | The Attribute of the modifier. |
| uuid | **invalid** | The unique identifier of the modifier to replace. |
| name | string | The name of the modifier. |
| value | double | The value of the modifier. |
| operation | [AttributeOperation](/vanilla/api/entity/attribute/AttributeOperation) | The operation of the modifier. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | What slots the modifier is valid for. |


:::

:::group{name=addGlobalAttributeModifier}

Adds an AttributeModifier to this IIngredient using a specific UUID.

 The UUID can be used to override an existing attribute on an ItemStack with this new modifier.
 You can use `/ct hand attributes` to get the UUID of the attributes on an ItemStack.

 Attributes added with this method appear on all ItemStacks that match this IIngredient,
 regardless of how or when the ItemStack was made, if you want to have the attribute on a
 single specific ItemStack (such as a specific Diamond Sword made in a recipe), then you should use
 IItemStack#withAttributeModifier

Return Type: void

```zenscript
// IngredientConditioned.addGlobalAttributeModifier(attribute as Attribute, uuid as string, name as string, value as double, operation as AttributeOperation, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.addGlobalAttributeModifier(<attribute:minecraft:generic.attack_damage>, "8c1b5535-9f79-448b-87ae-52d81480aaa3", "Extra Power", 10, AttributeOperation.ADDITION, [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| attribute | [Attribute](/vanilla/api/entity/attribute/Attribute) | The Attribute of the modifier. |
| uuid | string | The unique identifier of the modifier to replace. |
| name | string | The name of the modifier. |
| value | double | The value of the modifier. |
| operation | [AttributeOperation](/vanilla/api/entity/attribute/AttributeOperation) | The operation of the modifier. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | What slots the modifier is valid for. |


:::

:::group{name=addShiftTooltip}

Return Type: void

```zenscript
IngredientConditioned.addShiftTooltip(content as Component, showMessage as Component) as void
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| content | [Component](/vanilla/api/text/Component) | No Description Provided | false |  |
| showMessage | [Component](/vanilla/api/text/Component) | No Description Provided | true |  |


:::

:::group{name=addTooltip}

Return Type: void

```zenscript
IngredientConditioned.addTooltip(content as Component) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| content | [Component](/vanilla/api/text/Component) | No Description Provided |


:::

:::group{name=anyDamage}

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
// IngredientConditioned.anyDamage() as IngredientConditioned<IIngredient>

myIngredientConditioned.anyDamage();
```

:::

:::group{name=asIIngredientWithAmount}

Used implicitly when a machine can accept more than one item but you only provide one.

Return Type: [IIngredientWithAmount](/vanilla/api/ingredient/IIngredientWithAmount)

```zenscript
// IngredientConditioned.asIIngredientWithAmount() as IIngredientWithAmount

myIngredientConditioned.asIIngredientWithAmount();
```

:::

:::group{name=clearTooltip}

Return Type: void

```zenscript
IngredientConditioned.clearTooltip(leaveName as boolean) as void
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| leaveName | boolean | No Description Provided | true | false |


:::

:::group{name=contains}

Does the ingredient contain the given ingredient?

Return Type: boolean

```zenscript
// IngredientConditioned.contains(ingredient as IIngredient) as boolean

myIngredientConditioned.contains((<item:minecraft:iron_ingot> | <item:minecraft:gold_ingot>));
```

| Parameter | Type | Description |
|-----------|------|-------------|
| ingredient | [IIngredient](/vanilla/api/ingredient/IIngredient) | The ingredient to check |


:::

:::group{name=getRemainingItem}

When this ingredient stack is crafted, what will remain in the grid?
 Does not check if the stack matches though!
 Used e.g. in Crafting Table recipes.

Return Type: [IItemStack](/vanilla/api/item/IItemStack)

```zenscript
// IngredientConditioned.getRemainingItem(stack as IItemStack) as IItemStack

myIngredientConditioned.getRemainingItem(<item:minecraft:iron_ingot>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [IItemStack](/vanilla/api/item/IItemStack) | The stack to provide for this ingredient. |


:::

:::group{name=matches}

Does the given stack match the ingredient?

Return Type: boolean

```zenscript
// IngredientConditioned.matches(stack as IItemStack) as boolean

myIngredientConditioned.matches(<item:minecraft:iron_ingot>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [IItemStack](/vanilla/api/item/IItemStack) | The stack to check |


:::

:::group{name=matches}

Return Type: boolean

```zenscript
IngredientConditioned.matches(stack as IItemStack, ignoreDamage as boolean) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| stack | [IItemStack](/vanilla/api/item/IItemStack) | No Description Provided |
| ignoreDamage | boolean | No Description Provided |


:::

:::group{name=modifyShiftTooltip}

Return Type: void

```zenscript
IngredientConditioned.modifyShiftTooltip(shiftedFunction as ITooltipFunction, unshiftedFunction as ITooltipFunction) as void
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| shiftedFunction | [ITooltipFunction](/vanilla/api/item/tooltip/ITooltipFunction) | No Description Provided | false |  |
| unshiftedFunction | [ITooltipFunction](/vanilla/api/item/tooltip/ITooltipFunction) | No Description Provided | true |  |


:::

:::group{name=modifyTooltip}

Return Type: void

```zenscript
IngredientConditioned.modifyTooltip(function as ITooltipFunction) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| function | [ITooltipFunction](/vanilla/api/item/tooltip/ITooltipFunction) | No Description Provided |


:::

:::group{name=mul}

Use this in contexts where machines accept more than one item to state that fact.

Return Type: [IIngredientWithAmount](/vanilla/api/ingredient/IIngredientWithAmount)

```zenscript
IngredientConditioned.mul(amount as int) as IIngredientWithAmount
```

| Parameter | Type | Description |
|-----------|------|-------------|
| amount | int | No Description Provided |


:::

:::group{name=only}

Use this if you already have the condition from another ingredient

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.only(condition as IIngredientCondition<IIngredient>) as IngredientConditioned<IIngredient>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| condition | [IIngredientCondition](/vanilla/api/ingredient/condition/IIngredientCondition)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt; | No Description Provided |


:::

:::group{name=onlyDamaged}

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
// IngredientConditioned.onlyDamaged() as IngredientConditioned<IIngredient>

myIngredientConditioned.onlyDamaged();
```

:::

:::group{name=onlyDamagedAtLeast}

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.onlyDamagedAtLeast(minDamage as int) as IngredientConditioned<IIngredient>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| minDamage | int | No Description Provided |


:::

:::group{name=onlyDamagedAtMost}

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.onlyDamagedAtMost(maxDamage as int) as IngredientConditioned<IIngredient>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| maxDamage | int | No Description Provided |


:::

:::group{name=onlyIf}

Return Type: [IngredientConditioned](/vanilla/api/ingredient/type/IngredientConditioned)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.onlyIf(uid as string, function as Predicate<IItemStack>) as IngredientConditioned<IIngredient>
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| uid | string | No Description Provided | false |  |
| function | Predicate&lt;[IItemStack](/vanilla/api/item/IItemStack)&gt; | No Description Provided | true |  |


:::

:::group{name=removeGlobalAttribute}

Removes all AttributeModifiers that use the given Attribute from this IIngredient.

 Attributes removed with this method are removed from ItemStacks that match this IIngredient,
 regardless of how or when the ItemStack was made, if you want to remove the attribute on a
 single specific ItemStack (such as a specific Diamond Sword made in a recipe), then you should use
 IItemStack#withoutAttribute.

 This method can only remove default Attributes from an ItemStack, it is still possible that
 an ItemStack can override it.

Return Type: void

```zenscript
// IngredientConditioned.removeGlobalAttribute(attribute as Attribute, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.removeGlobalAttribute(<attribute:minecraft:generic.attack_damage>, [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| attribute | [Attribute](/vanilla/api/entity/attribute/Attribute) | The attribute to remove. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | The slot types to remove it from. |


:::

:::group{name=removeGlobalAttributeModifier}

Removes all AttributeModifiers who's ID is the same as the given uuid from this IIngredient.

Return Type: void

```zenscript
// IngredientConditioned.removeGlobalAttributeModifier(uuid as invalid, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.removeGlobalAttributeModifier(IItemStack.BASE_ATTACK_DAMAGE_UUID, [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| uuid | **invalid** | The unique id of the AttributeModifier to remove. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | The slot types to remove it from. |


:::

:::group{name=removeGlobalAttributeModifier}

Removes all AttributeModifiers who's ID is the same as the given uuid from this IIngredient.

Return Type: void

```zenscript
// IngredientConditioned.removeGlobalAttributeModifier(uuid as string, slotTypes as EquipmentSlot[]) as void

myIngredientConditioned.removeGlobalAttributeModifier("8c1b5535-9f79-448b-87ae-52d81480aaa3", [<constant:minecraft:equipmentslot:chest>]);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| uuid | string | The unique id of the AttributeModifier to remove. |
| slotTypes | [EquipmentSlot](/vanilla/api/entity/equipment/EquipmentSlot)[] | The slot types to remove it from. |


:::

:::group{name=removeTooltip}

Return Type: void

```zenscript
IngredientConditioned.removeTooltip(regex as string) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| regex | string | No Description Provided |


:::

:::group{name=reuse}

Return Type: [IIngredientTransformed](/vanilla/api/ingredient/type/IIngredientTransformed)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
// IngredientConditioned.reuse() as IIngredientTransformed<IIngredient>

myIngredientConditioned.reuse();
```

:::

:::group{name=setBurnTime}

Sets the burn time of this ingredient, for use in the furnace and other machines

Return Type: void

```zenscript
// IngredientConditioned.setBurnTime(time as int) as void

myIngredientConditioned.setBurnTime(500);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| time | int | the new burn time |


:::

:::group{name=transform}

Use this if you already have the transformer from another ingredient

Return Type: [IIngredientTransformed](/vanilla/api/ingredient/type/IIngredientTransformed)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.transform(transformer as IIngredientTransformer<IIngredient>) as IIngredientTransformed<IIngredient>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| transformer | [IIngredientTransformer](/vanilla/api/ingredient/transform/IIngredientTransformer)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt; | No Description Provided |


:::

:::group{name=transformCustom}

Return Type: [IIngredientTransformed](/vanilla/api/ingredient/type/IIngredientTransformed)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.transformCustom(uid as string, function as Function<IItemStack,IItemStack>) as IIngredientTransformed<IIngredient>
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| uid | string | No Description Provided | false |  |
| function | Function&lt;[IItemStack](/vanilla/api/item/IItemStack),[IItemStack](/vanilla/api/item/IItemStack)&gt; | No Description Provided | true |  |


:::

:::group{name=transformDamage}

Return Type: [IIngredientTransformed](/vanilla/api/ingredient/type/IIngredientTransformed)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.transformDamage(amount as int) as IIngredientTransformed<IIngredient>
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| amount | int | No Description Provided | true | 1 |


:::

:::group{name=transformReplace}

Return Type: [IIngredientTransformed](/vanilla/api/ingredient/type/IIngredientTransformed)&lt;[IIngredient](/vanilla/api/ingredient/IIngredient)&gt;

```zenscript
IngredientConditioned.transformReplace(replaceWith as IItemStack) as IIngredientTransformed<IIngredient>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| replaceWith | [IItemStack](/vanilla/api/item/IItemStack) | No Description Provided |


:::


## Operators

:::group{name=CONTAINS}

Does the ingredient contain the given ingredient?

```zenscript
ingredient as IIngredient in myIngredientConditioned
(<item:minecraft:iron_ingot> | <item:minecraft:gold_ingot>) in myIngredientConditioned
```

:::

:::group{name=MUL}

Use this in contexts where machines accept more than one item to state that fact.

```zenscript
myIngredientConditioned * amount as int
```

:::

:::group{name=OR}

```zenscript
myIngredientConditioned | other as IIngredient
```

:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| baseIngredient | T | true | false | No Description Provided |
| burnTime | void | false | true | Sets the burn time of this ingredient, for use in the furnace and other machines |
| condition | [IIngredientCondition](/vanilla/api/ingredient/condition/IIngredientCondition)&lt;T&gt; | true | false | No Description Provided |
| items | [IItemStack](/vanilla/api/item/IItemStack)[] | true | false | No Description Provided |

