# MobEffectInstance

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.entity.effect.MobEffectInstance;
```


## Implemented Interfaces
MobEffectInstance implements the following interfaces. That means all methods defined in these interfaces are also available in MobEffectInstance

- Comparable&lt;[MobEffectInstance](/vanilla/api/entity/effect/MobEffectInstance)&gt;

## Static Methods

:::group{name=load}

Return Type: [MobEffectInstance](/vanilla/api/entity/effect/MobEffectInstance)

```zenscript
MobEffectInstance.load(data as MapData) as MobEffectInstance
```

| Parameter | Type | Description |
|-----------|------|-------------|
| data | [MapData](/vanilla/api/data/MapData) | No Description Provided |


:::

## Constructors


```zenscript
new MobEffectInstance(mobEffect as MobEffect) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>);
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |



```zenscript
new MobEffectInstance(mobEffect as MobEffect, duration as int) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>, 100);
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |
| duration | int | No description provided |



```zenscript
new MobEffectInstance(mobEffect as MobEffect, duration as int, amplifier as int) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>, 100, 2);
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |
| duration | int | No description provided |
| amplifier | int | No description provided |



```zenscript
new MobEffectInstance(mobEffect as MobEffect, duration as int, amplifier as int, ambient as boolean, visible as boolean) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>, 100, 2, true, false);
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |
| duration | int | No description provided |
| amplifier | int | No description provided |
| ambient | boolean | No description provided |
| visible | boolean | No description provided |



```zenscript
new MobEffectInstance(mobEffect as MobEffect, duration as int, amplifier as int, ambient as boolean, visible as boolean, showIcon as boolean) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>, 100, 2, true, false, false);
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |
| duration | int | No description provided |
| amplifier | int | No description provided |
| ambient | boolean | No description provided |
| visible | boolean | No description provided |
| showIcon | boolean | No description provided |



```zenscript
new MobEffectInstance(mobEffect as MobEffect, duration as int, amplifier as int, ambient as boolean, visible as boolean, showIcon as boolean, hiddenEffect as MobEffectInstance) as MobEffectInstance
new MobEffectInstance(<mobeffect:minecraft:haste>, 100, 2, true, false, false, new MobEffectInstance(<mobeffect:minecraft:haste>, 200, 3));
```
| Parameter | Type | Description |
|-----------|------|-------------|
| mobEffect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | No description provided |
| duration | int | No description provided |
| amplifier | int | No description provided |
| ambient | boolean | No description provided |
| visible | boolean | No description provided |
| showIcon | boolean | No description provided |
| hiddenEffect | [MobEffectInstance](/vanilla/api/entity/effect/MobEffectInstance) | No description provided |



## Methods

:::group{name=applyEffect}

Return Type: void

```zenscript
MobEffectInstance.applyEffect(entity as LivingEntity) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| entity | [LivingEntity](/vanilla/api/entity/LivingEntity) | No Description Provided |


:::

:::group{name=compareTo}

Return Type: int

```zenscript
MobEffectInstance.compareTo(other as MobEffectInstance) as int
```

| Parameter | Type | Description |
|-----------|------|-------------|
| other | [MobEffectInstance](/vanilla/api/entity/effect/MobEffectInstance) | No Description Provided |


:::

:::group{name=getAmplifier}

Return Type: int

```zenscript
// MobEffectInstance.getAmplifier() as int

myMobEffectInstance.getAmplifier();
```

:::

:::group{name=getDescriptionId}

Return Type: string

```zenscript
// MobEffectInstance.getDescriptionId() as string

myMobEffectInstance.getDescriptionId();
```

:::

:::group{name=getDuration}

Return Type: int

```zenscript
// MobEffectInstance.getDuration() as int

myMobEffectInstance.getDuration();
```

:::

:::group{name=getEffect}

Return Type: [MobEffect](/vanilla/api/entity/effect/MobEffect)

```zenscript
// MobEffectInstance.getEffect() as MobEffect

myMobEffectInstance.getEffect();
```

:::

:::group{name=isAmbient}

Return Type: boolean

```zenscript
// MobEffectInstance.isAmbient() as boolean

myMobEffectInstance.isAmbient();
```

:::

:::group{name=isNoCounter}

Return Type: boolean

```zenscript
// MobEffectInstance.isNoCounter() as boolean

myMobEffectInstance.isNoCounter();
```

:::

:::group{name=isVisible}

Return Type: boolean

```zenscript
// MobEffectInstance.isVisible() as boolean

myMobEffectInstance.isVisible();
```

:::

:::group{name=save}

Return Type: [MapData](/vanilla/api/data/MapData)

```zenscript
MobEffectInstance.save(data as MapData) as MapData
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| data | [MapData](/vanilla/api/data/MapData) | No Description Provided | true |  |


:::

:::group{name=setNoCounter}

Return Type: void

```zenscript
MobEffectInstance.setNoCounter(noCounter as boolean) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| noCounter | boolean | No Description Provided |


:::

:::group{name=showIcon}

Return Type: boolean

```zenscript
// MobEffectInstance.showIcon() as boolean

myMobEffectInstance.showIcon();
```

:::

:::group{name=tick}

Return Type: boolean

```zenscript
MobEffectInstance.tick(entity as LivingEntity, onFinish as invalid) as boolean
```

| Parameter | Type | Description | Optional | DefaultValue |
|-----------|------|-------------|----------|--------------|
| entity | [LivingEntity](/vanilla/api/entity/LivingEntity) | No Description Provided | false |  |
| onFinish | **invalid** | No Description Provided | true | null |


:::

:::group{name=update}

Return Type: boolean

```zenscript
MobEffectInstance.update(instance as MobEffectInstance) as boolean
```

| Parameter | Type | Description |
|-----------|------|-------------|
| instance | [MobEffectInstance](/vanilla/api/entity/effect/MobEffectInstance) | No Description Provided |


:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| ambient | boolean | true | false | No Description Provided |
| amplifier | int | true | false | No Description Provided |
| descriptionId | string | true | false | No Description Provided |
| duration | int | true | false | No Description Provided |
| effect | [MobEffect](/vanilla/api/entity/effect/MobEffect) | true | false | No Description Provided |
| isNoCounter | boolean | true | false | No Description Provided |
| showIcon | boolean | true | false | No Description Provided |
| visible | boolean | true | false | No Description Provided |

