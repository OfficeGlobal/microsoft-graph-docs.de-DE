---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8fafb266b2bfc2c7ea6e0951ac2906f133817246
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860977"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="d4cbc-103">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d4cbc-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="d4cbc-104">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4cbc-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4cbc-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4cbc-105">Properties</span></span>

| <span data-ttu-id="d4cbc-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4cbc-106">Property</span></span>            | <span data-ttu-id="d4cbc-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d4cbc-107">Type</span></span>     | <span data-ttu-id="d4cbc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4cbc-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d4cbc-109">id</span><span class="sxs-lookup"><span data-stu-id="d4cbc-109">id</span></span>                  | <span data-ttu-id="d4cbc-110">string</span><span class="sxs-lookup"><span data-stu-id="d4cbc-110">string</span></span>   | <span data-ttu-id="d4cbc-111">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="d4cbc-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="d4cbc-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="d4cbc-112">teamsAppId</span></span>          | <span data-ttu-id="d4cbc-113">string</span><span class="sxs-lookup"><span data-stu-id="d4cbc-113">string</span></span>   | <span data-ttu-id="d4cbc-114">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="d4cbc-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="d4cbc-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d4cbc-115">displayName</span></span>         | <span data-ttu-id="d4cbc-116">string</span><span class="sxs-lookup"><span data-stu-id="d4cbc-116">string</span></span>   | <span data-ttu-id="d4cbc-117">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="d4cbc-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="d4cbc-118">Version</span><span class="sxs-lookup"><span data-stu-id="d4cbc-118">version</span></span>             | <span data-ttu-id="d4cbc-119">string</span><span class="sxs-lookup"><span data-stu-id="d4cbc-119">string</span></span>   | <span data-ttu-id="d4cbc-120">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="d4cbc-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4cbc-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4cbc-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d4cbc-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d4cbc-122">See also</span></span>

- [<span data-ttu-id="d4cbc-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d4cbc-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d4cbc-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d4cbc-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d4cbc-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d4cbc-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

