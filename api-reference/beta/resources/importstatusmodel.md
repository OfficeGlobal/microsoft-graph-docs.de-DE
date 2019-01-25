---
title: Ressourcentyp importStatusModel
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: c3fe64245d0fbce98db3ba87c3c39694e998c7e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526053"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="00b93-103">Ressourcentyp importStatusModel</span><span class="sxs-lookup"><span data-stu-id="00b93-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="00b93-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00b93-104">JSON representation</span></span>

<span data-ttu-id="00b93-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00b93-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="00b93-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00b93-106">Properties</span></span>
| <span data-ttu-id="00b93-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00b93-107">Property</span></span>     | <span data-ttu-id="00b93-108">Typ</span><span class="sxs-lookup"><span data-stu-id="00b93-108">Type</span></span>   |<span data-ttu-id="00b93-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00b93-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00b93-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00b93-110">createdDateTime</span></span>| <span data-ttu-id="00b93-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00b93-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="00b93-112">id</span><span class="sxs-lookup"><span data-stu-id="00b93-112">id</span></span>|<span data-ttu-id="00b93-113">string</span><span class="sxs-lookup"><span data-stu-id="00b93-113">string</span></span>||
|<span data-ttu-id="00b93-114">status</span><span class="sxs-lookup"><span data-stu-id="00b93-114">status</span></span>|<span data-ttu-id="00b93-115">string</span><span class="sxs-lookup"><span data-stu-id="00b93-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/importstatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
