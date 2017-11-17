---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: 61fc7c117d2da961b1b6d581e21db27d7afe3f31
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="3c599-102">GeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c599-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="3c599-p101">Die **GeoCoordinates**-Ressource liefert geografische Koordinaten und die Erhebung eines Orts basierend auf Metadaten, die in der Datei enthalten sind. Wenn ein [**DriveItem**](driveitem.md) ein **location**-Facet ungleich Null aufweist, stellt das Element eine Datei dar, die mit einem bekannten Ort verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="3c599-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c599-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c599-105">JSON representation</span></span>

<span data-ttu-id="3c599-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c599-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c599-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c599-107">Properties</span></span>

| <span data-ttu-id="3c599-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c599-108">Property</span></span>  | <span data-ttu-id="3c599-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3c599-109">Type</span></span>   | <span data-ttu-id="3c599-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c599-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="3c599-111">altitude</span><span class="sxs-lookup"><span data-stu-id="3c599-111">altitude</span></span>  | <span data-ttu-id="3c599-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="3c599-112">Double</span></span> | <span data-ttu-id="3c599-p102">Optional. Die Höhe oberhalb des Meeresspiegels in Fuß. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c599-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="3c599-116">latitude</span><span class="sxs-lookup"><span data-stu-id="3c599-116">latitude</span></span>  | <span data-ttu-id="3c599-117">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="3c599-117">Double</span></span> | <span data-ttu-id="3c599-p103">Optional. Der Breitengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c599-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="3c599-121">longitude</span><span class="sxs-lookup"><span data-stu-id="3c599-121">longitude</span></span> | <span data-ttu-id="3c599-122">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="3c599-122">Double</span></span> | <span data-ttu-id="3c599-p104">Optional. Der Längengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3c599-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="3c599-126">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="3c599-126">Remarks</span></span>

<span data-ttu-id="3c599-127">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c599-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
