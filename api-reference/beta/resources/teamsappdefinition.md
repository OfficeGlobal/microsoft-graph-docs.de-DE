---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94e2c790f8bf4623e56ca76bde164b718ee6fa38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509980"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="719d6-103">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="719d6-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="719d6-104">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="719d6-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="719d6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="719d6-105">Properties</span></span>

| <span data-ttu-id="719d6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="719d6-106">Property</span></span>            | <span data-ttu-id="719d6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="719d6-107">Type</span></span>     | <span data-ttu-id="719d6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="719d6-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="719d6-109">id</span><span class="sxs-lookup"><span data-stu-id="719d6-109">id</span></span>                  | <span data-ttu-id="719d6-110">string</span><span class="sxs-lookup"><span data-stu-id="719d6-110">string</span></span>   | <span data-ttu-id="719d6-111">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="719d6-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="719d6-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="719d6-112">teamsAppId</span></span>          | <span data-ttu-id="719d6-113">string</span><span class="sxs-lookup"><span data-stu-id="719d6-113">string</span></span>   | <span data-ttu-id="719d6-114">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="719d6-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="719d6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="719d6-115">displayName</span></span>         | <span data-ttu-id="719d6-116">string</span><span class="sxs-lookup"><span data-stu-id="719d6-116">string</span></span>   | <span data-ttu-id="719d6-117">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="719d6-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="719d6-118">Version</span><span class="sxs-lookup"><span data-stu-id="719d6-118">version</span></span>             | <span data-ttu-id="719d6-119">string</span><span class="sxs-lookup"><span data-stu-id="719d6-119">string</span></span>   | <span data-ttu-id="719d6-120">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="719d6-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="719d6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="719d6-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="719d6-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="719d6-122">See also</span></span>

- [<span data-ttu-id="719d6-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="719d6-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="719d6-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="719d6-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="719d6-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="719d6-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

