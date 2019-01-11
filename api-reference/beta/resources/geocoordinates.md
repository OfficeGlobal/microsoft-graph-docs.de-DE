---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852640"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="5c151-102">GeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5c151-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="5c151-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5c151-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c151-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c151-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c151-p102">Die **GeoCoordinates**-Ressource liefert geografische Koordinaten und die Erhebung eines Orts basierend auf Metadaten, die in der Datei enthalten sind. Wenn ein [**DriveItem**](driveitem.md) ein **location**-Facet ungleich Null aufweist, stellt das Element eine Datei dar, die mit einem bekannten Ort verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="5c151-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c151-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5c151-107">JSON representation</span></span>

<span data-ttu-id="5c151-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5c151-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="5c151-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5c151-109">Properties</span></span>

| <span data-ttu-id="5c151-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c151-110">Property</span></span>  | <span data-ttu-id="5c151-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5c151-111">Type</span></span>   | <span data-ttu-id="5c151-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c151-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="5c151-113">altitude</span><span class="sxs-lookup"><span data-stu-id="5c151-113">altitude</span></span>  | <span data-ttu-id="5c151-114">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="5c151-114">Double</span></span> | <span data-ttu-id="5c151-p103">Optional. Die Höhe oberhalb des Meeresspiegels in Fuß. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5c151-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="5c151-118">latitude</span><span class="sxs-lookup"><span data-stu-id="5c151-118">latitude</span></span>  | <span data-ttu-id="5c151-119">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="5c151-119">Double</span></span> | <span data-ttu-id="5c151-p104">Optional. Der Breitengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5c151-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="5c151-123">longitude</span><span class="sxs-lookup"><span data-stu-id="5c151-123">longitude</span></span> | <span data-ttu-id="5c151-124">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="5c151-124">Double</span></span> | <span data-ttu-id="5c151-p105">Optional. Der Längengrad für das Element als Kommazahl. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5c151-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="5c151-128">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="5c151-128">Remarks</span></span>

<span data-ttu-id="5c151-129">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5c151-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
