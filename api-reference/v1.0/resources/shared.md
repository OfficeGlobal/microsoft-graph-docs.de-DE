---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Geteilt
ms.openlocfilehash: 1d828310a226edd0443ff3b5f60156df1e7c98cb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="shared-resource-type"></a><span data-ttu-id="95283-102">Shared-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="95283-102">Shared resource type</span></span>

<span data-ttu-id="95283-103">Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="95283-103">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>
<span data-ttu-id="95283-104">Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.</span><span class="sxs-lookup"><span data-stu-id="95283-104">The Shared resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="95283-105">Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="95283-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95283-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95283-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="95283-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95283-107">Properties</span></span>

| <span data-ttu-id="95283-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95283-108">Property</span></span>       | <span data-ttu-id="95283-109">Typ</span><span class="sxs-lookup"><span data-stu-id="95283-109">Type</span></span>                          | <span data-ttu-id="95283-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95283-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="95283-111">owner</span><span class="sxs-lookup"><span data-stu-id="95283-111">owner</span></span>          | [<span data-ttu-id="95283-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="95283-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="95283-p102">Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="95283-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="95283-115">scope</span><span class="sxs-lookup"><span data-stu-id="95283-115">scope</span></span>          | <span data-ttu-id="95283-116">String</span><span class="sxs-lookup"><span data-stu-id="95283-116">String</span></span>                        | <span data-ttu-id="95283-117">Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`.</span><span class="sxs-lookup"><span data-stu-id="95283-117">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`.</span></span> <span data-ttu-id="95283-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="95283-118">Read-only.</span></span>
| <span data-ttu-id="95283-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="95283-119">sharedBy</span></span>       | [<span data-ttu-id="95283-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="95283-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="95283-p104">Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="95283-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="95283-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="95283-123">sharedDateTime</span></span> | <span data-ttu-id="95283-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95283-124">DateTimeOffset</span></span>                | <span data-ttu-id="95283-p105">UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="95283-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="95283-127">Bereichswerte</span><span class="sxs-lookup"><span data-stu-id="95283-127">Scope values</span></span>

| <span data-ttu-id="95283-128">Wert</span><span class="sxs-lookup"><span data-stu-id="95283-128">Value</span></span>          | <span data-ttu-id="95283-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95283-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="95283-130">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.</span><span class="sxs-lookup"><span data-stu-id="95283-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="95283-131">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert.</span><span class="sxs-lookup"><span data-stu-id="95283-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="95283-132">Das Element wird nur für bestimmte Benutzern freigegeben.</span><span class="sxs-lookup"><span data-stu-id="95283-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="95283-133">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="95283-133">Remarks</span></span>

<span data-ttu-id="95283-134">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="95283-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
