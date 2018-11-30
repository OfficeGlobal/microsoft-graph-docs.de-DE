---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
ms.openlocfilehash: f61d37eecccd4bf08a2f8abbf4cda15dee5eb94d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062025"
---
# <a name="photo-resource-type"></a><span data-ttu-id="97811-102">Photo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="97811-102">Photo resource type</span></span>

> <span data-ttu-id="97811-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97811-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97811-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97811-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97811-105">Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="97811-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="97811-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97811-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="97811-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97811-107">Properties</span></span>

| <span data-ttu-id="97811-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97811-108">Property</span></span>                | <span data-ttu-id="97811-109">Typ</span><span class="sxs-lookup"><span data-stu-id="97811-109">Type</span></span>           | <span data-ttu-id="97811-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97811-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="97811-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="97811-111">**takenDateTime**</span></span>       | <span data-ttu-id="97811-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97811-112">DateTimeOffset</span></span> | <span data-ttu-id="97811-p102">Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="97811-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="97811-115">**cameraMake**</span></span>          | <span data-ttu-id="97811-116">String</span><span class="sxs-lookup"><span data-stu-id="97811-116">String</span></span>         | <span data-ttu-id="97811-p103">Kamerahersteller Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="97811-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="97811-119">**cameraModel**</span></span>         | <span data-ttu-id="97811-120">String</span><span class="sxs-lookup"><span data-stu-id="97811-120">String</span></span>         | <span data-ttu-id="97811-p104">Kameramodell. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="97811-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="97811-123">**fNumber**</span></span>             | <span data-ttu-id="97811-124">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="97811-124">Double</span></span>         | <span data-ttu-id="97811-p105">Die Blendenzahl der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="97811-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="97811-127">**exposureDenominator**</span></span> | <span data-ttu-id="97811-128">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="97811-128">Double</span></span>         | <span data-ttu-id="97811-p106">Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="97811-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="97811-131">**exposureNumerator**</span></span>   | <span data-ttu-id="97811-132">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="97811-132">Double</span></span>         | <span data-ttu-id="97811-p107">Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="97811-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="97811-135">**focalLength**</span></span>         | <span data-ttu-id="97811-136">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="97811-136">Double</span></span>         | <span data-ttu-id="97811-p108">Die Brennweite der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="97811-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="97811-139">**iso**</span></span>                 | <span data-ttu-id="97811-140">Int64</span><span class="sxs-lookup"><span data-stu-id="97811-140">Int64</span></span>          | <span data-ttu-id="97811-p109">Der ISO-Wert der Kamera. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97811-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="97811-143">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="97811-143">Remarks</span></span>
<span data-ttu-id="97811-144">Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97811-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="97811-145">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="97811-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
