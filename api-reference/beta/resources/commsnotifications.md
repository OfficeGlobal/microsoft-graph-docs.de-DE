---
title: Ressourcentyp commsNotifications
description: Liste der Benachrichtigungen für mehrere Benachrichtigungen gesendet werden in einem einzelnen Batch von den Communications-Servern verwendet.
author: VinodRavichandran
ms.openlocfilehash: 052520a99081e5c09cd6e3ec3b74f74e9527d38d
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380450"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="a68b6-103">Ressourcentyp commsNotifications</span><span class="sxs-lookup"><span data-stu-id="a68b6-103">commsNotifications resource type</span></span>

> <span data-ttu-id="a68b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a68b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a68b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a68b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a68b6-106">Liste der Benachrichtigungen für mehrere Benachrichtigungen gesendet werden in einem einzelnen Batch von den Communications-Servern verwendet.</span><span class="sxs-lookup"><span data-stu-id="a68b6-106">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="a68b6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a68b6-107">Properties</span></span>

| <span data-ttu-id="a68b6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a68b6-108">Property</span></span>       | <span data-ttu-id="a68b6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a68b6-109">Type</span></span>                                                 | <span data-ttu-id="a68b6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a68b6-110">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="a68b6-111">Wert</span><span class="sxs-lookup"><span data-stu-id="a68b6-111">value</span></span>          | <span data-ttu-id="a68b6-112">[CommsNotification](commsnotification.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a68b6-112">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="a68b6-113">Die Benachrichtigung über eine Änderung in der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a68b6-113">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a68b6-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a68b6-114">JSON representation</span></span>

<span data-ttu-id="a68b6-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a68b6-115">The following is a JSON representation of the resource.</span></span>

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
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->