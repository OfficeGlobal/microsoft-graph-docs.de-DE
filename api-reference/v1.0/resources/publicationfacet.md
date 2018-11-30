---
title: PublicationFacet-Ressourcentyp
description: Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer DriveItemVersion- oder DriveItem-Ressource.
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016581"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="801af-103">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="801af-103">PublicationFacet resource type</span></span>

<span data-ttu-id="801af-104">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="801af-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="801af-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="801af-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="801af-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="801af-106">Properties</span></span>

|   <span data-ttu-id="801af-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="801af-107">Property</span></span>    |  <span data-ttu-id="801af-108">Typ</span><span class="sxs-lookup"><span data-stu-id="801af-108">Type</span></span>  | <span data-ttu-id="801af-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="801af-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="801af-110">**level**</span><span class="sxs-lookup"><span data-stu-id="801af-110">**level**</span></span>     | <span data-ttu-id="801af-111">string</span><span class="sxs-lookup"><span data-stu-id="801af-111">String</span></span> | <span data-ttu-id="801af-112">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="801af-112">The state of publication for this document.</span></span> <span data-ttu-id="801af-113">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="801af-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="801af-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="801af-114">Read-only.</span></span>  |
| <span data-ttu-id="801af-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="801af-115">**versionId**</span></span> | <span data-ttu-id="801af-116">string</span><span class="sxs-lookup"><span data-stu-id="801af-116">String</span></span> | <span data-ttu-id="801af-117">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="801af-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="801af-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="801af-118">Read-only.</span></span>  |


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
