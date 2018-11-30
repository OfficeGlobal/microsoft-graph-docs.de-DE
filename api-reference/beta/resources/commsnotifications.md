---
title: Benachrichtigungen Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065832"
---
# <a name="notifications-resource-type"></a><span data-ttu-id="88eb7-103">Benachrichtigungen Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88eb7-103">notifications resource type</span></span>

> <span data-ttu-id="88eb7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88eb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88eb7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88eb7-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="88eb7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88eb7-106">Properties</span></span>

| <span data-ttu-id="88eb7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88eb7-107">Property</span></span>       | <span data-ttu-id="88eb7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="88eb7-108">Type</span></span>                                       | <span data-ttu-id="88eb7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88eb7-109">Description</span></span> |
|:---------------|:-------------------------------------------|:------------|
| <span data-ttu-id="88eb7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="88eb7-110">value</span></span>          | <span data-ttu-id="88eb7-111">[Benachrichtigung](commsnotification.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="88eb7-111">[notification](commsnotification.md) collection</span></span> | <span data-ttu-id="88eb7-112">Die Benachrichtigung über eine Änderung in der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88eb7-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88eb7-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88eb7-113">JSON representation</span></span>

<span data-ttu-id="88eb7-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88eb7-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->