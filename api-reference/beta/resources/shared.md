---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Geteilt
ms.openlocfilehash: 38bc8604ba2528a24e2193a2fb521428b2b5c2d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063888"
---
# <a name="shared-resource-type"></a><span data-ttu-id="8dd37-102">Shared-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8dd37-102">Shared resource type</span></span>

> <span data-ttu-id="8dd37-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8dd37-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dd37-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8dd37-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dd37-p102">Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde. Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.</span><span class="sxs-lookup"><span data-stu-id="8dd37-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="8dd37-107">Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="8dd37-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dd37-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dd37-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8dd37-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8dd37-109">Properties</span></span>

| <span data-ttu-id="8dd37-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8dd37-110">Property</span></span>       | <span data-ttu-id="8dd37-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8dd37-111">Type</span></span>                          | <span data-ttu-id="8dd37-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dd37-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="8dd37-113">owner</span><span class="sxs-lookup"><span data-stu-id="8dd37-113">owner</span></span>          | [<span data-ttu-id="8dd37-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8dd37-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="8dd37-p103">Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8dd37-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="8dd37-117">Bereich</span><span class="sxs-lookup"><span data-stu-id="8dd37-117">scope</span></span>          | <span data-ttu-id="8dd37-118">String</span><span class="sxs-lookup"><span data-stu-id="8dd37-118">String</span></span>                        | <span data-ttu-id="8dd37-p104">Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8dd37-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="8dd37-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="8dd37-121">sharedBy</span></span>       | [<span data-ttu-id="8dd37-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="8dd37-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="8dd37-p105">Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8dd37-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="8dd37-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dd37-125">sharedDateTime</span></span> | <span data-ttu-id="8dd37-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dd37-126">DateTimeOffset</span></span>                | <span data-ttu-id="8dd37-p106">UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8dd37-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="8dd37-129">Bereichswerte</span><span class="sxs-lookup"><span data-stu-id="8dd37-129">Scope values</span></span>

| <span data-ttu-id="8dd37-130">Wert</span><span class="sxs-lookup"><span data-stu-id="8dd37-130">Value</span></span>          | <span data-ttu-id="8dd37-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dd37-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="8dd37-132">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.</span><span class="sxs-lookup"><span data-stu-id="8dd37-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="8dd37-133">Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert.</span><span class="sxs-lookup"><span data-stu-id="8dd37-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="8dd37-134">Das Element wird nur für bestimmte Benutzern freigegeben.</span><span class="sxs-lookup"><span data-stu-id="8dd37-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="8dd37-135">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="8dd37-135">Remarks</span></span>

<span data-ttu-id="8dd37-136">Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8dd37-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
