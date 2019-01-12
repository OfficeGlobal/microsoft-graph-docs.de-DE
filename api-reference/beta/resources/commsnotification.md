---
title: Ressourcentyp commsNotification
description: Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e5b929997cf17d13043264d42421418321aae84e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977696"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="08b56-103">Ressourcentyp commsNotification</span><span class="sxs-lookup"><span data-stu-id="08b56-103">commsNotification resource type</span></span>

> <span data-ttu-id="08b56-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08b56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08b56-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08b56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08b56-106">Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="08b56-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="08b56-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08b56-107">Properties</span></span>
| <span data-ttu-id="08b56-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08b56-108">Property</span></span>       | <span data-ttu-id="08b56-109">Typ</span><span class="sxs-lookup"><span data-stu-id="08b56-109">Type</span></span>    | <span data-ttu-id="08b56-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08b56-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="08b56-111">changeType</span><span class="sxs-lookup"><span data-stu-id="08b56-111">changeType</span></span>     | <span data-ttu-id="08b56-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b56-112">String</span></span>  | <span data-ttu-id="08b56-113">Mögliche Werte sind: `created`, `updated` und `deleted`.</span><span class="sxs-lookup"><span data-stu-id="08b56-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="08b56-114">resource</span><span class="sxs-lookup"><span data-stu-id="08b56-114">resource</span></span>       | <span data-ttu-id="08b56-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08b56-115">String</span></span>  | <span data-ttu-id="08b56-116">Der URI der Ressource, die geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="08b56-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="08b56-117">**Hinweis:** `resourceData` als zusätzliche Daten verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="08b56-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="08b56-118">Es ist eine Entität oder Collection(entity) abhängig von der Anzahl der Änderungen in der Benachrichtigung gepackt.</span><span class="sxs-lookup"><span data-stu-id="08b56-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08b56-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08b56-119">JSON representation</span></span>

<span data-ttu-id="08b56-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08b56-120">The following is a JSON representation of the resource.</span></span>

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
