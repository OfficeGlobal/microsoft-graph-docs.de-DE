# <a name="photo-resource-type"></a><span data-ttu-id="c3acc-101">Photo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3acc-101">Photo resource type</span></span>

<span data-ttu-id="c3acc-102">Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="c3acc-102">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3acc-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3acc-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="c3acc-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3acc-104">Properties</span></span>
| <span data-ttu-id="c3acc-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3acc-105">Property</span></span>                | <span data-ttu-id="c3acc-106">Typ</span><span class="sxs-lookup"><span data-stu-id="c3acc-106">Type</span></span>                      | <span data-ttu-id="c3acc-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3acc-107">Description</span></span>                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| <span data-ttu-id="c3acc-108">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="c3acc-108">**takenDateTime**</span></span>       | <span data-ttu-id="c3acc-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3acc-109">DateTimeOffset</span></span>            | <span data-ttu-id="c3acc-p101">Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p101">Represents the date and time the photo was taken. Read-only.</span></span>               |
| <span data-ttu-id="c3acc-112">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="c3acc-112">**cameraMake**</span></span>          | <span data-ttu-id="c3acc-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3acc-113">String</span></span>                    | <span data-ttu-id="c3acc-p102">Kamerahersteller Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p102">Camera manufacturer. Read-only.</span></span>                                            |
| <span data-ttu-id="c3acc-116">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="c3acc-116">**cameraModel**</span></span>         | <span data-ttu-id="c3acc-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3acc-117">String</span></span>                    | <span data-ttu-id="c3acc-p103">Kameramodell. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p103">Camera model. Read-only.</span></span>                                                   |
| <span data-ttu-id="c3acc-120">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="c3acc-120">**fNumber**</span></span>             | <span data-ttu-id="c3acc-121">Double</span><span class="sxs-lookup"><span data-stu-id="c3acc-121">Double</span></span>                    | <span data-ttu-id="c3acc-p104">Die Blendenzahl der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p104">The F-stop value from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="c3acc-124">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="c3acc-124">**exposureDenominator**</span></span> | <span data-ttu-id="c3acc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c3acc-125">Int32</span></span>                     | <span data-ttu-id="c3acc-p105">Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
| <span data-ttu-id="c3acc-128">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="c3acc-128">**exposureNumerator**</span></span>   | <span data-ttu-id="c3acc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c3acc-129">Int32</span></span>                     | <span data-ttu-id="c3acc-p106">Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
| <span data-ttu-id="c3acc-132">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="c3acc-132">**focalLength**</span></span>         | <span data-ttu-id="c3acc-133">Double</span><span class="sxs-lookup"><span data-stu-id="c3acc-133">Double</span></span>                    | <span data-ttu-id="c3acc-p107">Die Brennweite der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p107">The focal length from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="c3acc-136">**iso**</span><span class="sxs-lookup"><span data-stu-id="c3acc-136">**iso**</span></span>                 | <span data-ttu-id="c3acc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c3acc-137">Int32</span></span>                     | <span data-ttu-id="c3acc-p108">Der ISO-Wert der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3acc-p108">The ISO value from the camera. Read-only.</span></span>                                  |

## <a name="remarks"></a><span data-ttu-id="c3acc-140">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="c3acc-140">Remarks</span></span>
<span data-ttu-id="c3acc-141">Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3acc-141">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="c3acc-142">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c3acc-142">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
