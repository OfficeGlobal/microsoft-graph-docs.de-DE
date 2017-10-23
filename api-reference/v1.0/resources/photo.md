---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a><span data-ttu-id="c5cf8-102">Photo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c5cf8-102">Photo resource type</span></span>

<span data-ttu-id="c5cf8-103">Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5cf8-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5cf8-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="c5cf8-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5cf8-105">Properties</span></span>

| <span data-ttu-id="c5cf8-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5cf8-106">Property</span></span>                | <span data-ttu-id="c5cf8-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c5cf8-107">Type</span></span>           | <span data-ttu-id="c5cf8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5cf8-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="c5cf8-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-109">**takenDateTime**</span></span>       | <span data-ttu-id="c5cf8-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5cf8-110">DateTimeOffset</span></span> | <span data-ttu-id="c5cf8-p101">Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="c5cf8-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-113">**cameraMake**</span></span>          | <span data-ttu-id="c5cf8-114">String</span><span class="sxs-lookup"><span data-stu-id="c5cf8-114">String</span></span>         | <span data-ttu-id="c5cf8-p102">Kamerahersteller Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="c5cf8-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-117">**cameraModel**</span></span>         | <span data-ttu-id="c5cf8-118">String</span><span class="sxs-lookup"><span data-stu-id="c5cf8-118">String</span></span>         | <span data-ttu-id="c5cf8-p103">Kameramodell. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="c5cf8-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-121">**fNumber**</span></span>             | <span data-ttu-id="c5cf8-122">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="c5cf8-122">Double</span></span>         | <span data-ttu-id="c5cf8-p104">Die Blendenzahl der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="c5cf8-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-125">**exposureDenominator**</span></span> | <span data-ttu-id="c5cf8-126">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="c5cf8-126">Double</span></span>         | <span data-ttu-id="c5cf8-p105">Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="c5cf8-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-129">**exposureNumerator**</span></span>   | <span data-ttu-id="c5cf8-130">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="c5cf8-130">Double</span></span>         | <span data-ttu-id="c5cf8-p106">Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="c5cf8-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-133">**focalLength**</span></span>         | <span data-ttu-id="c5cf8-134">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="c5cf8-134">Double</span></span>         | <span data-ttu-id="c5cf8-p107">Die Brennweite der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="c5cf8-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="c5cf8-137">**iso**</span></span>                 | <span data-ttu-id="c5cf8-138">Int64</span><span class="sxs-lookup"><span data-stu-id="c5cf8-138">Int64</span></span>          | <span data-ttu-id="c5cf8-p108">Der ISO-Wert der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="c5cf8-141">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="c5cf8-141">Remarks</span></span>
<span data-ttu-id="c5cf8-142">Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5cf8-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="c5cf8-143">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c5cf8-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
