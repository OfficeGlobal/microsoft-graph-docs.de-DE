---
title: Benachrichtigung Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: c09927cbe133c945b83a3bfc1b0eb74ef00bce2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064597"
---
# <a name="notification-resource-type"></a><span data-ttu-id="cca03-103">Benachrichtigung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cca03-103">notification resource type</span></span>

> <span data-ttu-id="cca03-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cca03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cca03-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cca03-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="cca03-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cca03-106">Properties</span></span>
| <span data-ttu-id="cca03-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cca03-107">Property</span></span>       | <span data-ttu-id="cca03-108">Typ</span><span class="sxs-lookup"><span data-stu-id="cca03-108">Type</span></span>    | <span data-ttu-id="cca03-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cca03-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="cca03-110">changeType</span><span class="sxs-lookup"><span data-stu-id="cca03-110">changeType</span></span>     | <span data-ttu-id="cca03-111">String</span><span class="sxs-lookup"><span data-stu-id="cca03-111">String</span></span>  | <span data-ttu-id="cca03-112">Mögliche Werte sind: `created`, `updated` und `deleted`.</span><span class="sxs-lookup"><span data-stu-id="cca03-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="cca03-113">resource</span><span class="sxs-lookup"><span data-stu-id="cca03-113">resource</span></span>       | <span data-ttu-id="cca03-114">String</span><span class="sxs-lookup"><span data-stu-id="cca03-114">String</span></span>  | <span data-ttu-id="cca03-115">Der URI der Ressource, die geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="cca03-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="cca03-116">**Hinweis:** `resourceData` als zusätzliche Daten verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="cca03-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="cca03-117">Es ist eine Entität oder Collection(entity) abhängig von der Anzahl der Änderungen in der Benachrichtigung gepackt.</span><span class="sxs-lookup"><span data-stu-id="cca03-117">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cca03-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cca03-118">JSON representation</span></span>

<span data-ttu-id="cca03-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cca03-119">The following is a JSON representation of the resource.</span></span>

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
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->