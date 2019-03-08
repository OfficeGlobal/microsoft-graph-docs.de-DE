---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482063"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="9d4ad-102">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9d4ad-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d4ad-103">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d4ad-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d4ad-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d4ad-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d4ad-105">Properties</span></span>

|   <span data-ttu-id="9d4ad-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d4ad-106">Property</span></span>    |  <span data-ttu-id="9d4ad-107">Typ</span><span class="sxs-lookup"><span data-stu-id="9d4ad-107">Type</span></span>  | <span data-ttu-id="9d4ad-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d4ad-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="9d4ad-109">**level**</span><span class="sxs-lookup"><span data-stu-id="9d4ad-109">**level**</span></span>     | <span data-ttu-id="9d4ad-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d4ad-110">String</span></span> | <span data-ttu-id="9d4ad-111">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-111">The state of publication for this document.</span></span> <span data-ttu-id="9d4ad-112">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="9d4ad-113">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-113">Read-only.</span></span>  |
| <span data-ttu-id="9d4ad-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="9d4ad-114">**versionId**</span></span> | <span data-ttu-id="9d4ad-115">string</span><span class="sxs-lookup"><span data-stu-id="9d4ad-115">String</span></span> | <span data-ttu-id="9d4ad-116">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="9d4ad-117">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9d4ad-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
