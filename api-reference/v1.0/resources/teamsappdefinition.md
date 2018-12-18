---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
ms.openlocfilehash: 43bd4262008a29668739e78d4b598da1e77e3d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351639"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="341b0-103">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="341b0-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="341b0-104">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="341b0-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="341b0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="341b0-105">Properties</span></span>

| <span data-ttu-id="341b0-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="341b0-106">Property</span></span>            | <span data-ttu-id="341b0-107">Typ</span><span class="sxs-lookup"><span data-stu-id="341b0-107">Type</span></span>     | <span data-ttu-id="341b0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="341b0-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="341b0-109">id</span><span class="sxs-lookup"><span data-stu-id="341b0-109">id</span></span>                  | <span data-ttu-id="341b0-110">string</span><span class="sxs-lookup"><span data-stu-id="341b0-110">string</span></span>   | <span data-ttu-id="341b0-111">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="341b0-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="341b0-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="341b0-112">teamsAppId</span></span>          | <span data-ttu-id="341b0-113">string</span><span class="sxs-lookup"><span data-stu-id="341b0-113">string</span></span>   | <span data-ttu-id="341b0-114">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="341b0-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="341b0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="341b0-115">displayName</span></span>         | <span data-ttu-id="341b0-116">string</span><span class="sxs-lookup"><span data-stu-id="341b0-116">string</span></span>   | <span data-ttu-id="341b0-117">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="341b0-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="341b0-118">Version</span><span class="sxs-lookup"><span data-stu-id="341b0-118">version</span></span>             | <span data-ttu-id="341b0-119">string</span><span class="sxs-lookup"><span data-stu-id="341b0-119">string</span></span>   | <span data-ttu-id="341b0-120">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="341b0-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="341b0-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="341b0-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="341b0-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="341b0-122">See also</span></span>

- [<span data-ttu-id="341b0-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="341b0-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="341b0-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="341b0-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="341b0-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="341b0-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

