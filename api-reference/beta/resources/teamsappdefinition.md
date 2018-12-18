---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
ms.openlocfilehash: 71a1783131661aed120f375f7cc58d55fb0ca0d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336834"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="d2be0-103">Ressourcentyp teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d2be0-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="d2be0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d2be0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2be0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2be0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2be0-106">Die Details einer Version von einer [TeamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2be0-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2be0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2be0-107">Properties</span></span>

| <span data-ttu-id="d2be0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2be0-108">Property</span></span>            | <span data-ttu-id="d2be0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d2be0-109">Type</span></span>     | <span data-ttu-id="d2be0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2be0-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d2be0-111">id</span><span class="sxs-lookup"><span data-stu-id="d2be0-111">id</span></span>                  | <span data-ttu-id="d2be0-112">string</span><span class="sxs-lookup"><span data-stu-id="d2be0-112">string</span></span>   | <span data-ttu-id="d2be0-113">Eine eindeutige Id (nicht die Teams Appid).</span><span class="sxs-lookup"><span data-stu-id="d2be0-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="d2be0-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="d2be0-114">teamsAppId</span></span>          | <span data-ttu-id="d2be0-115">string</span><span class="sxs-lookup"><span data-stu-id="d2be0-115">string</span></span>   | <span data-ttu-id="d2be0-116">Die Id von Teams App-Manifest.</span><span class="sxs-lookup"><span data-stu-id="d2be0-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="d2be0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="d2be0-117">displayName</span></span>         | <span data-ttu-id="d2be0-118">string</span><span class="sxs-lookup"><span data-stu-id="d2be0-118">string</span></span>   | <span data-ttu-id="d2be0-119">Der Name der app bereitgestellt von der app-Entwickler.</span><span class="sxs-lookup"><span data-stu-id="d2be0-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="d2be0-120">Version</span><span class="sxs-lookup"><span data-stu-id="d2be0-120">version</span></span>             | <span data-ttu-id="d2be0-121">string</span><span class="sxs-lookup"><span data-stu-id="d2be0-121">string</span></span>   | <span data-ttu-id="d2be0-122">Die Versionsnummer der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="d2be0-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2be0-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2be0-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d2be0-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d2be0-124">See also</span></span>

- [<span data-ttu-id="d2be0-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d2be0-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d2be0-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d2be0-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d2be0-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d2be0-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

