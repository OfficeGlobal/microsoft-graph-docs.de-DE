---
title: Ressourcentyp organizerMeetingInfo
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 00a7978c44c82ddd6b34802f29188a554e7e0b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062012"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="c43d7-103">Ressourcentyp organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="c43d7-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="c43d7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c43d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c43d7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c43d7-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="c43d7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c43d7-106">Properties</span></span>

| <span data-ttu-id="c43d7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c43d7-107">Property</span></span>                     | <span data-ttu-id="c43d7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c43d7-108">Type</span></span>                          | <span data-ttu-id="c43d7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43d7-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="c43d7-110">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="c43d7-110">allowConversationWithoutHost</span></span> | <span data-ttu-id="c43d7-111">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c43d7-111">Boolean</span></span>                       | <span data-ttu-id="c43d7-112">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="c43d7-112">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="c43d7-113">organizer</span><span class="sxs-lookup"><span data-stu-id="c43d7-113">organizer</span></span>                    | [<span data-ttu-id="c43d7-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c43d7-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="c43d7-115">Der Organisator Azure Active Directory-Identität.</span><span class="sxs-lookup"><span data-stu-id="c43d7-115">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c43d7-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c43d7-116">JSON representation</span></span>

<span data-ttu-id="c43d7-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c43d7-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="c43d7-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c43d7-118">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
