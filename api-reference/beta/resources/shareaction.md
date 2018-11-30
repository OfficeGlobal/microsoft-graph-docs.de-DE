---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
ms.openlocfilehash: c9f06c7a4a6351b8a6554c944c0efe9af379e030
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062316"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="5aada-102">ShareAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5aada-102">ShareAction resource type</span></span>

> <span data-ttu-id="5aada-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5aada-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5aada-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5aada-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5aada-105">Die **ShareAction**-Ressource enthält Informationen zu einer [Aktivität][activity], die ein Element freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="5aada-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5aada-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5aada-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5aada-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5aada-107">Properties</span></span>

| <span data-ttu-id="5aada-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="5aada-108">Property name</span></span> | <span data-ttu-id="5aada-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5aada-109">Type</span></span>                       | <span data-ttu-id="5aada-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aada-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="5aada-111">recipients</span><span class="sxs-lookup"><span data-stu-id="5aada-111">recipients</span></span>    | <span data-ttu-id="5aada-112">[IdentitySet][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5aada-112">[identitySet][] collection</span></span> | <span data-ttu-id="5aada-113">Die Identitäten, für die das Element in der Aktion freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="5aada-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="5aada-115">Hinweise</span><span class="sxs-lookup"><span data-stu-id="5aada-115">Remarks</span></span>

<span data-ttu-id="5aada-116">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5aada-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
