---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: af426d5e51f87b9fd8894c6e956947cc75f1a38d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481797"
---
# <a name="shared-resource-type"></a><span data-ttu-id="6d7b4-102">Shared-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6d7b4-102">Shared resource type</span></span>

<span data-ttu-id="6d7b4-p101">Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde. Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="6d7b4-105">Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d7b4-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d7b4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6d7b4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d7b4-107">Properties</span></span>

| <span data-ttu-id="6d7b4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d7b4-108">Property</span></span>       | <span data-ttu-id="6d7b4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6d7b4-109">Type</span></span>                          | <span data-ttu-id="6d7b4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d7b4-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="6d7b4-111">owner</span><span class="sxs-lookup"><span data-stu-id="6d7b4-111">owner</span></span>          | [<span data-ttu-id="6d7b4-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6d7b4-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="6d7b4-p102">Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="6d7b4-115">scope</span><span class="sxs-lookup"><span data-stu-id="6d7b4-115">scope</span></span>          | <span data-ttu-id="6d7b4-116">String</span><span class="sxs-lookup"><span data-stu-id="6d7b4-116">String</span></span>                        | <span data-ttu-id="6d7b4-p103">Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="6d7b4-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="6d7b4-119">sharedBy</span></span>       | [<span data-ttu-id="6d7b4-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d7b4-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="6d7b4-p104">Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="6d7b4-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d7b4-123">sharedDateTime</span></span> | <span data-ttu-id="6d7b4-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d7b4-124">DateTimeOffset</span></span>                | <span data-ttu-id="6d7b4-p105">UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="6d7b4-127">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="6d7b4-127">Scope options</span></span>

| <span data-ttu-id="6d7b4-128">Wert</span><span class="sxs-lookup"><span data-stu-id="6d7b4-128">Value</span></span>          | <span data-ttu-id="6d7b4-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d7b4-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="6d7b4-130">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="6d7b4-131">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="6d7b4-132">Das Element wird nur für bestimmte Benutzern freigegeben.</span><span class="sxs-lookup"><span data-stu-id="6d7b4-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="6d7b4-133">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="6d7b4-133">Remarks</span></span>

<span data-ttu-id="6d7b4-134">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6d7b4-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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
