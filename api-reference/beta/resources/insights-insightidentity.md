---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 47283a82260d4f03a271a16660d58aca60da94e1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577227"
---
# <a name="insightidentity"></a><span data-ttu-id="5f107-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="5f107-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f107-104">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="5f107-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="5f107-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f107-105">JSON representation</span></span>
<span data-ttu-id="5f107-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f107-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5f107-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f107-107">Properties</span></span>

| <span data-ttu-id="5f107-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f107-108">Property</span></span>              | <span data-ttu-id="5f107-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5f107-109">Type</span></span>          | <span data-ttu-id="5f107-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f107-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="5f107-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5f107-111">displayName</span></span>       | <span data-ttu-id="5f107-112">String</span><span class="sxs-lookup"><span data-stu-id="5f107-112">String</span></span>          | <span data-ttu-id="5f107-113">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="5f107-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="5f107-114">id</span><span class="sxs-lookup"><span data-stu-id="5f107-114">id</span></span>              | <span data-ttu-id="5f107-115">String</span><span class="sxs-lookup"><span data-stu-id="5f107-115">String</span></span>        | <span data-ttu-id="5f107-116">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="5f107-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="5f107-117">address</span><span class="sxs-lookup"><span data-stu-id="5f107-117">address</span></span>             | <span data-ttu-id="5f107-118">String</span><span class="sxs-lookup"><span data-stu-id="5f107-118">String</span></span>      | <span data-ttu-id="5f107-119">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f107-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
