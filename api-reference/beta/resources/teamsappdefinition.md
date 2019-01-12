---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 312b9347519935c4ff34f51cee24e0082c3da58e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969765"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="66d9a-103">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="66d9a-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="66d9a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66d9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66d9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66d9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66d9a-106">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="66d9a-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66d9a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66d9a-107">Properties</span></span>

| <span data-ttu-id="66d9a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66d9a-108">Property</span></span>            | <span data-ttu-id="66d9a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="66d9a-109">Type</span></span>     | <span data-ttu-id="66d9a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66d9a-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="66d9a-111">id</span><span class="sxs-lookup"><span data-stu-id="66d9a-111">id</span></span>                  | <span data-ttu-id="66d9a-112">string</span><span class="sxs-lookup"><span data-stu-id="66d9a-112">string</span></span>   | <span data-ttu-id="66d9a-113">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="66d9a-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="66d9a-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="66d9a-114">teamsAppId</span></span>          | <span data-ttu-id="66d9a-115">string</span><span class="sxs-lookup"><span data-stu-id="66d9a-115">string</span></span>   | <span data-ttu-id="66d9a-116">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="66d9a-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="66d9a-117">displayName</span><span class="sxs-lookup"><span data-stu-id="66d9a-117">displayName</span></span>         | <span data-ttu-id="66d9a-118">string</span><span class="sxs-lookup"><span data-stu-id="66d9a-118">string</span></span>   | <span data-ttu-id="66d9a-119">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="66d9a-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="66d9a-120">Version</span><span class="sxs-lookup"><span data-stu-id="66d9a-120">version</span></span>             | <span data-ttu-id="66d9a-121">string</span><span class="sxs-lookup"><span data-stu-id="66d9a-121">string</span></span>   | <span data-ttu-id="66d9a-122">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="66d9a-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66d9a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66d9a-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="66d9a-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="66d9a-124">See also</span></span>

- [<span data-ttu-id="66d9a-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66d9a-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="66d9a-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="66d9a-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="66d9a-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66d9a-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

