---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 16bc590fcfe14f9ce7f6f1bbe38492225cce099c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828658"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="54141-102">ShareAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="54141-102">ShareAction resource type</span></span>

> <span data-ttu-id="54141-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54141-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54141-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54141-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54141-105">Die **ShareAction**-Ressource enthält Informationen zu einer [Aktivität][activity], die ein Element freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="54141-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="54141-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54141-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="54141-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54141-107">Properties</span></span>

| <span data-ttu-id="54141-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="54141-108">Property name</span></span> | <span data-ttu-id="54141-109">Typ</span><span class="sxs-lookup"><span data-stu-id="54141-109">Type</span></span>                       | <span data-ttu-id="54141-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54141-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="54141-111">recipients</span><span class="sxs-lookup"><span data-stu-id="54141-111">recipients</span></span>    | <span data-ttu-id="54141-112">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="54141-112">[identitySet][] collection</span></span> | <span data-ttu-id="54141-113">Die Identitäten, für die das Element in der Aktion freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="54141-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="54141-115">Hinweise</span><span class="sxs-lookup"><span data-stu-id="54141-115">Remarks</span></span>

<span data-ttu-id="54141-116">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="54141-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
