# AdvancementRewards

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.advancement.AdvancementRewards;
```


## Methods

:::group{name=getRecipes}

Return Type: [ResourceLocation](/vanilla/api/resource/ResourceLocation)[]

```zenscript
// AdvancementRewards.getRecipes() as ResourceLocation[]

myAdvancementRewards.getRecipes();
```

:::

:::group{name=grant}

Return Type: void

```zenscript
AdvancementRewards.grant(player as ServerPlayer) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| player | [ServerPlayer](/vanilla/api/entity/type/player/ServerPlayer) | No Description Provided |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| recipes | [ResourceLocation](/vanilla/api/resource/ResourceLocation)[] | true | false | No Description Provided |

