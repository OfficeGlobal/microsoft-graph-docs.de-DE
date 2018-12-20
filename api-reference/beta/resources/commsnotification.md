---
title: Ressourcentyp commsNotification
description: Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.
author: VinodRavichandran
ms.openlocfilehash: 65cb2884b98d25008779fcb80968a7b4d0481033
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380268"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="41b8b-103">Ressourcentyp commsNotification</span><span class="sxs-lookup"><span data-stu-id="41b8b-103">commsNotification resource type</span></span>

> <span data-ttu-id="41b8b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="41b8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41b8b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41b8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41b8b-106">Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="41b8b-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="41b8b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41b8b-107">Properties</span></span>
| <span data-ttu-id="41b8b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41b8b-108">Property</span></span>       | <span data-ttu-id="41b8b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="41b8b-109">Type</span></span>    | <span data-ttu-id="41b8b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41b8b-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="41b8b-111">changeType</span><span class="sxs-lookup"><span data-stu-id="41b8b-111">changeType</span></span>     | <span data-ttu-id="41b8b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41b8b-112">String</span></span>  | <span data-ttu-id="41b8b-113">Mögliche Werte sind: `created`, `updated` und `deleted`.</span><span class="sxs-lookup"><span data-stu-id="41b8b-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="41b8b-114">resource</span><span class="sxs-lookup"><span data-stu-id="41b8b-114">resource</span></span>       | <span data-ttu-id="41b8b-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41b8b-115">String</span></span>  | <span data-ttu-id="41b8b-116">Der URI der Ressource, die geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="41b8b-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="41b8b-117">**Hinweis:** `resourceData` als zusätzliche Daten verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="41b8b-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="41b8b-118">Es ist eine Entität oder Collection(entity) abhängig von der Anzahl der Änderungen in der Benachrichtigung gepackt.</span><span class="sxs-lookup"><span data-stu-id="41b8b-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41b8b-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41b8b-119">JSON representation</span></span>

<span data-ttu-id="41b8b-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41b8b-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->