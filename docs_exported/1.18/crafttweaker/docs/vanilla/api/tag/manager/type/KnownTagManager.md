# KnownTagManager&LT;T : Object&GT;

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.tag.manager.type.KnownTagManager;
```


## Implemented Interfaces
KnownTagManager implements the following interfaces. That means all methods defined in these interfaces are also available in KnownTagManager

- [ITagManager](/vanilla/api/tag/manager/ITagManager)&lt;[KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;&gt;

## Methods

:::group{name=addElements}

Return Type: void

```zenscript
KnownTagManager.addElements(to as KnownTag<T>, values as T[]) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| to | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt; | No Description Provided |
| values | T[] | No Description Provided |


:::

:::group{name=elements}

Gets the elements of the given tag.

Returns: The list of elements in the tag.  
Return Type: stdlib.List&lt;T&gt;

```zenscript
// KnownTagManager.elements(of as KnownTag<T>) as stdlib.List<T>

myKnownTagManager.elements(<tag:items:minecraft:dirt>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| of | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt; | The tag to get the elements of. |


:::

:::group{name=exists}

Checks if a tag with the given id exists and is registered.

Returns: true if it exists, false otherwise.  
Return Type: boolean

```zenscript
// KnownTagManager.exists(id as ResourceLocation) as boolean

myKnownTagManager.exists(<resource:minecraft:wool>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| id | [ResourceLocation](/vanilla/api/resource/ResourceLocation) | The id of the tag to check. |


:::

:::group{name=exists}

Checks if a tag with the given id exists and is registered.

Returns: true if it exists, false otherwise.  
Return Type: boolean

```zenscript
// KnownTagManager.exists(id as string) as boolean

myKnownTagManager.exists("minecraft:wool");
```

| Parameter | Type | Description |
|-----------|------|-------------|
| id | string | The id of the tag to check. |


:::

:::group{name=exists}

Checks if the given tag exists and is registered.

Returns: true if it exists, false otherwise.  
Return Type: boolean

```zenscript
// KnownTagManager.exists(tag as T) as boolean

myKnownTagManager.exists(<tag:items:minecraft:wool>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| tag | T | The tag to check. |


:::

:::group{name=getTagsFor}

Ges the tags that contain the given element.

Returns: The tags that contain the given elements.  
Return Type: stdlib.List&lt;T&gt;

```zenscript
KnownTagManager.getTagsFor(element as ResourceLocation) as stdlib.List<T>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| element | [ResourceLocation](/vanilla/api/resource/ResourceLocation) | No Description Provided |


:::

:::group{name=getTagsFor}

Return Type: stdlib.List&lt;[KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;&gt;

```zenscript
KnownTagManager.getTagsFor(element as T) as stdlib.List<KnownTag<T>>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| element | T | No Description Provided |


:::

:::group{name=idElements}

Gets the [ResourceLocation](/vanilla/api/resource/ResourceLocation) ids of the elements in the given tag.

Returns: A List of [ResourceLocation](/vanilla/api/resource/ResourceLocation) ids of the elements in the given tag.  
Return Type: stdlib.List&lt;[ResourceLocation](/vanilla/api/resource/ResourceLocation)&gt;

```zenscript
// KnownTagManager.idElements(of as T) as stdlib.List<ResourceLocation>

myKnownTagManager.idElements(<tag:items:minecraft:wool>);
```

| Parameter | Type | Description |
|-----------|------|-------------|
| of | T | The tag to get the elements of. |


:::

:::group{name=removeElements}

Return Type: void

```zenscript
KnownTagManager.removeElements(from as KnownTag<T>, values as T[]) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| from | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt; | No Description Provided |
| values | T[] | No Description Provided |


:::

:::group{name=removeId}

Return Type: void

```zenscript
KnownTagManager.removeId(from as KnownTag<T>, values as ResourceLocation[]) as void
```

| Parameter | Type | Description |
|-----------|------|-------------|
| from | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt; | No Description Provided |
| values | [ResourceLocation](/vanilla/api/resource/ResourceLocation)[] | No Description Provided |


:::

:::group{name=tag}

Return Type: [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;

```zenscript
KnownTagManager.tag(id as ResourceLocation) as KnownTag<T>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| id | [ResourceLocation](/vanilla/api/resource/ResourceLocation) | No Description Provided |


:::

:::group{name=tag}

Return Type: [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;

```zenscript
KnownTagManager.tag(id as string) as KnownTag<T>
```

| Parameter | Type | Description |
|-----------|------|-------------|
| id | string | No Description Provided |


:::

:::group{name=tagFolder}

Gets the tagFolder of this manager.

 The tag folder is usually the folder on disk without the `tags/` prefix.

 Examples:
 <ul>
 <li>`tags/items` turns into `items`</li>
 <li>`tags/potion` turns into `potion`</li>
 <li>`tags/worldgen/biome` turns into `worldgen/biome`</li>
 </ul>

Returns: The tag folder of this manager.  
Return Type: string

```zenscript
// KnownTagManager.tagFolder() as string

myKnownTagManager.tagFolder();
```

:::

:::group{name=tagMap}

Return Type: [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;[[ResourceLocation](/vanilla/api/resource/ResourceLocation)]

```zenscript
// KnownTagManager.tagMap() as KnownTag<T>[ResourceLocation]

myKnownTagManager.tagMap();
```

:::

:::group{name=tags}

Ges the tags that this manager knows about.

Returns: The tags that this manager knows about.  
Return Type: stdlib.List&lt;T&gt;

```zenscript
// KnownTagManager.tags() as stdlib.List<T>

myKnownTagManager.tags();
```

:::


## Operators

:::group{name=CONTAINS}

Checks if a tag with the given id exists and is registered.

```zenscript
id as string in myKnownTagManager
"minecraft:wool" in myKnownTagManager
```

:::


## Properties

| Name | Type | Has Getter | Has Setter | Description |
|------|------|------------|------------|-------------|
| tagFolder | string | true | false | Gets the tagFolder of this manager. <br />  <br />  The tag folder is usually the folder on disk without the `tags/` prefix. <br />  <br />  Examples: <br />  <ul> <br />  <li>`tags/items` turns into `items`</li> <br />  <li>`tags/potion` turns into `potion`</li> <br />  <li>`tags/worldgen/biome` turns into `worldgen/biome`</li> <br />  </ul> |
| tagMap | [KnownTag](/vanilla/api/tag/type/KnownTag)&lt;T&gt;[[ResourceLocation](/vanilla/api/resource/ResourceLocation)] | true | false | No Description Provided |
| tags | stdlib.List&lt;T&gt; | true | false | Ges the tags that this manager knows about. |

