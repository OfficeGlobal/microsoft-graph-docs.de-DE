---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Geteilt
localization_priority: Normal
ms.openlocfilehash: 3478a8911a402bf86a04f196d87409e7cddb246e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868075"
---
# <a name="shared-resource-type"></a><span data-ttu-id="2e79a-102">Shared-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e79a-102">Shared resource type</span></span>

<span data-ttu-id="2e79a-p101">Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde. Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.</span><span class="sxs-lookup"><span data-stu-id="2e79a-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="2e79a-105">Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="2e79a-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e79a-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e79a-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="2e79a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e79a-107">Properties</span></span>

| <span data-ttu-id="2e79a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e79a-108">Property</span></span>       | <span data-ttu-id="2e79a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2e79a-109">Type</span></span>                          | <span data-ttu-id="2e79a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e79a-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="2e79a-111">owner</span><span class="sxs-lookup"><span data-stu-id="2e79a-111">owner</span></span>          | [<span data-ttu-id="2e79a-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2e79a-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="2e79a-p102">Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e79a-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="2e79a-115">scope</span><span class="sxs-lookup"><span data-stu-id="2e79a-115">scope</span></span>          | <span data-ttu-id="2e79a-116">String</span><span class="sxs-lookup"><span data-stu-id="2e79a-116">String</span></span>                        | <span data-ttu-id="2e79a-p103">Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e79a-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="2e79a-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="2e79a-119">sharedBy</span></span>       | [<span data-ttu-id="2e79a-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="2e79a-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="2e79a-p104">Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e79a-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="2e79a-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e79a-123">sharedDateTime</span></span> | <span data-ttu-id="2e79a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e79a-124">DateTimeOffset</span></span>                | <span data-ttu-id="2e79a-p105">UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e79a-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="2e79a-127">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="2e79a-127">Scope options</span></span>

| <span data-ttu-id="2e79a-128">Wert</span><span class="sxs-lookup"><span data-stu-id="2e79a-128">Value</span></span>          | <span data-ttu-id="2e79a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e79a-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="2e79a-130">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.</span><span class="sxs-lookup"><span data-stu-id="2e79a-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="2e79a-131">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert.</span><span class="sxs-lookup"><span data-stu-id="2e79a-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="2e79a-132">Das Element wird nur für bestimmte Benutzern freigegeben.</span><span class="sxs-lookup"><span data-stu-id="2e79a-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="2e79a-133">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="2e79a-133">Remarks</span></span>

<span data-ttu-id="2e79a-134">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2e79a-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->
