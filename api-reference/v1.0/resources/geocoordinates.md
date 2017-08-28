# <a name="geocoordinates-resource-type"></a><span data-ttu-id="73785-101">GeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73785-101">GeoCoordinates resource type</span></span>

<span data-ttu-id="73785-p101">Die **GeoCoordinates**-Ressource liefert geografische Koordinaten und die Erhebung eines Orts basierend auf Metadaten, die in der Datei enthalten sind. Wenn ein [**DriveItem**](driveitem.md) ein **location**-Facet ungleich Null aufweist, stellt das Element eine Datei dar, die mit einem bekannten Ort verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="73785-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73785-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73785-104">JSON representation</span></span>

<span data-ttu-id="73785-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73785-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="73785-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73785-106">Properties</span></span>

| <span data-ttu-id="73785-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73785-107">Property</span></span>  | <span data-ttu-id="73785-108">Typ</span><span class="sxs-lookup"><span data-stu-id="73785-108">Type</span></span>   | <span data-ttu-id="73785-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73785-109">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="73785-110">altitude</span><span class="sxs-lookup"><span data-stu-id="73785-110">altitude</span></span>  | <span data-ttu-id="73785-111">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="73785-111">Double</span></span> | <span data-ttu-id="73785-p102">Optional. Die Höhe oberhalb des Meeresspiegels in Fuß. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73785-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span> |
| <span data-ttu-id="73785-115">latitude</span><span class="sxs-lookup"><span data-stu-id="73785-115">latitude</span></span>  | <span data-ttu-id="73785-116">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="73785-116">Double</span></span> | <span data-ttu-id="73785-p103">Optional. Der Breitengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73785-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>   |
| <span data-ttu-id="73785-120">longitude</span><span class="sxs-lookup"><span data-stu-id="73785-120">longitude</span></span> | <span data-ttu-id="73785-121">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="73785-121">Double</span></span> | <span data-ttu-id="73785-p104">Optional. Der Längengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73785-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="73785-125">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="73785-125">Remarks</span></span>

<span data-ttu-id="73785-126">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="73785-126">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
