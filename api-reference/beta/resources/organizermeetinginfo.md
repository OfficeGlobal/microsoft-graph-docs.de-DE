---
title: Ressourcentyp organizerMeetingInfo
description: Besprechungsinformationen, die den Organisator der Besprechung enthält.
author: VinodRavichandran
ms.openlocfilehash: 296b20125908caf73221c2a8380e91931deb7e61
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380212"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="5f9bf-103">Ressourcentyp organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="5f9bf-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="5f9bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f9bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f9bf-106">Besprechungsinformationen, die den Organisator der Besprechung enthält.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="5f9bf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f9bf-107">Properties</span></span>

| <span data-ttu-id="5f9bf-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f9bf-108">Property</span></span>                     | <span data-ttu-id="5f9bf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5f9bf-109">Type</span></span>                          | <span data-ttu-id="5f9bf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f9bf-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="5f9bf-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="5f9bf-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="5f9bf-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5f9bf-112">Boolean</span></span>                       | <span data-ttu-id="5f9bf-113">Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="5f9bf-114">organizer</span><span class="sxs-lookup"><span data-stu-id="5f9bf-114">organizer</span></span>                    | [<span data-ttu-id="5f9bf-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="5f9bf-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="5f9bf-116">Der Organisator Azure Active Directory-Identität.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5f9bf-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f9bf-117">JSON representation</span></span>

<span data-ttu-id="5f9bf-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f9bf-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="5f9bf-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f9bf-119">Example</span></span>

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
