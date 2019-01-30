---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643888"
---
# <a name="insightidentity"></a><span data-ttu-id="8eb52-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="8eb52-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eb52-104">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="8eb52-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="8eb52-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8eb52-105">JSON representation</span></span>
<span data-ttu-id="8eb52-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8eb52-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8eb52-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8eb52-107">Properties</span></span>

| <span data-ttu-id="8eb52-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8eb52-108">Property</span></span>              | <span data-ttu-id="8eb52-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8eb52-109">Type</span></span>          | <span data-ttu-id="8eb52-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eb52-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="8eb52-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb52-111">displayName</span></span>       | <span data-ttu-id="8eb52-112">String</span><span class="sxs-lookup"><span data-stu-id="8eb52-112">String</span></span>          | <span data-ttu-id="8eb52-113">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="8eb52-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="8eb52-114">id</span><span class="sxs-lookup"><span data-stu-id="8eb52-114">id</span></span>              | <span data-ttu-id="8eb52-115">String</span><span class="sxs-lookup"><span data-stu-id="8eb52-115">String</span></span>        | <span data-ttu-id="8eb52-116">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="8eb52-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="8eb52-117">address</span><span class="sxs-lookup"><span data-stu-id="8eb52-117">address</span></span>             | <span data-ttu-id="8eb52-118">String</span><span class="sxs-lookup"><span data-stu-id="8eb52-118">String</span></span>      | <span data-ttu-id="8eb52-119">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="8eb52-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
