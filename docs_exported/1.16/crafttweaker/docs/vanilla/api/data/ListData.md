# ListData



## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.data.ListData;
```


## Implemented Interfaces
ListData implements the following interfaces. That means all methods defined in these interfaces are also available in ListData

- [ICollectionData](/vanilla/api/data/ICollectionData)

## Constructors

No Description Provided
```zenscript
new ListData() as ListData
new ListData();
```
No Description Provided
```zenscript
new ListData(list as stdlib.List<IData>) as ListData
```
| Parameter | Type | Description |
|-----------|------|-------------|
| list | stdlib.List&lt;[IData](/vanilla/api/data/IData)&gt; | No Description Provided |



## Casters

| Result type | Is Implicit |
|-------------|-------------|
| boolean | false |
| [ICollectionData](/vanilla/api/data/ICollectionData) | false |
| [INumberData](/vanilla/api/data/INumberData) | false |
| stdlib.List&lt;[IData](/vanilla/api/data/IData)&gt; | true |

## Methods

:::group{name=asBoolean}

Return Type: boolean

```zenscript
// ListData.asBoolean() as boolean

["Hello", "World", "!"].asBoolean();
```

:::

:::group{name=asCollection}

Return Type: [ICollectionData](/vanilla/api/data/ICollectionData)

```zenscript
// ListData.asCollection() as ICollectionData

["Hello", "World", "!"].asCollection();
```

:::

:::group{name=asFormattedText}

Return Type: [MCTextComponent](/vanilla/api/util/text/MCTextComponent)

```zenscript
ListData.asFormattedText(indentation as string, indentDepth as int) as MCTextComponent
```

| Parameter | Type | Description |
|-----------|------|-------------|
| indentation | string | No Description Provided |
| indentDepth | int | No Description Provided |


:::

:::group{name=asMap}

Gets a Map<String, IData> representation of this IData, returns null on anything but [MapData](/vanilla/api/data/MapData).

Returns: null if this IData is not a map.  
Return Type: [IData](/vanilla/api/data/IData)[string]

```zenscript
// ListData.asMap() as IData[string]

["Hello", "World", "!"].asMap();
```

:::

:::group{name=asNumber}

Return Type: [INumberData](/vanilla/api/data/INumberData)

```zenscript
// ListData.asNumber() as INumberData

["Hello", "World", "!"].asNumber();
```

:::

:::group{name=getData}

Return Type: T

```zenscript
ListData.getData<T : IData>(index as int) as T
```

| Parameter | Type | Description |
|-----------|------|-------------|
| index | int | No Description Provided |
| T | [IData](/vanilla/api/data/IData) | No Description Provided |


:::

:::group{name=getId}

Gets the ID of the internal NBT tag.

 Used to determine what NBT type is stored (in a list for example)

Returns: ID of the NBT tag that this data represents.  
Return Type: byte

```zenscript
// ListData.getId() as byte

["Hello", "World", "!"].getId();
```

:::

:::group{name=getString}

Gets the String representation of the internal INBT tag

Returns: String that represents the internal INBT of this IData.  
Return Type: string

```zenscript
// ListData.getString() as string

["Hello", "World", "!"].getString();
```

:::


