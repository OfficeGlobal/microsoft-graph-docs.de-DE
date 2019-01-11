---
title: PublicationFacet-Ressourcentyp
description: Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer DriveItemVersion- oder DriveItem-Ressource.
localization_priority: Normal
ms.openlocfilehash: 3d722f56cf1d587483c672fb7a1b7c05abd3671b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810528"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="5815a-103">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5815a-103">PublicationFacet resource type</span></span>

<span data-ttu-id="5815a-104">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="5815a-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5815a-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5815a-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5815a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5815a-106">Properties</span></span>

|   <span data-ttu-id="5815a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5815a-107">Property</span></span>    |  <span data-ttu-id="5815a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5815a-108">Type</span></span>  | <span data-ttu-id="5815a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5815a-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="5815a-110">**level**</span><span class="sxs-lookup"><span data-stu-id="5815a-110">**level**</span></span>     | <span data-ttu-id="5815a-111">string</span><span class="sxs-lookup"><span data-stu-id="5815a-111">String</span></span> | <span data-ttu-id="5815a-112">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="5815a-112">The state of publication for this document.</span></span> <span data-ttu-id="5815a-113">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="5815a-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="5815a-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5815a-114">Read-only.</span></span>  |
| <span data-ttu-id="5815a-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="5815a-115">**versionId**</span></span> | <span data-ttu-id="5815a-116">string</span><span class="sxs-lookup"><span data-stu-id="5815a-116">String</span></span> | <span data-ttu-id="5815a-117">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="5815a-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="5815a-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5815a-118">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
