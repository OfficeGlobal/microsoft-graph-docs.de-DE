---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: ed891f917ba8018aac349976df0455adfd269fdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869384"
---
# <a name="photo-resource-type"></a><span data-ttu-id="7b632-102">Photo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7b632-102">Photo resource type</span></span>

> <span data-ttu-id="7b632-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b632-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b632-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b632-105">Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="7b632-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b632-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7b632-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7b632-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7b632-107">Properties</span></span>

| <span data-ttu-id="7b632-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b632-108">Property</span></span>                | <span data-ttu-id="7b632-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7b632-109">Type</span></span>           | <span data-ttu-id="7b632-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b632-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="7b632-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="7b632-111">**takenDateTime**</span></span>       | <span data-ttu-id="7b632-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b632-112">DateTimeOffset</span></span> | <span data-ttu-id="7b632-p102">Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="7b632-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="7b632-115">**cameraMake**</span></span>          | <span data-ttu-id="7b632-116">String</span><span class="sxs-lookup"><span data-stu-id="7b632-116">String</span></span>         | <span data-ttu-id="7b632-p103">Kamerahersteller Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="7b632-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="7b632-119">**cameraModel**</span></span>         | <span data-ttu-id="7b632-120">String</span><span class="sxs-lookup"><span data-stu-id="7b632-120">String</span></span>         | <span data-ttu-id="7b632-p104">Kameramodell. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="7b632-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="7b632-123">**fNumber**</span></span>             | <span data-ttu-id="7b632-124">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="7b632-124">Double</span></span>         | <span data-ttu-id="7b632-p105">Die Blendenzahl der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="7b632-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="7b632-127">**exposureDenominator**</span></span> | <span data-ttu-id="7b632-128">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="7b632-128">Double</span></span>         | <span data-ttu-id="7b632-p106">Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="7b632-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="7b632-131">**exposureNumerator**</span></span>   | <span data-ttu-id="7b632-132">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="7b632-132">Double</span></span>         | <span data-ttu-id="7b632-p107">Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="7b632-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="7b632-135">**focalLength**</span></span>         | <span data-ttu-id="7b632-136">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="7b632-136">Double</span></span>         | <span data-ttu-id="7b632-p108">Die Brennweite der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="7b632-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="7b632-139">**iso**</span></span>                 | <span data-ttu-id="7b632-140">Int64</span><span class="sxs-lookup"><span data-stu-id="7b632-140">Int64</span></span>          | <span data-ttu-id="7b632-p109">Der ISO-Wert der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b632-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="7b632-143">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7b632-143">Remarks</span></span>
<span data-ttu-id="7b632-144">Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b632-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="7b632-145">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7b632-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
