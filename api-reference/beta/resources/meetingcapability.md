---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
author: VinodRavichandran
ms.openlocfilehash: 1a6f172922c0efbc9ad93e32141e364e2d0fc711
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380247"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="fffa2-103">Ressourcentyp meetingCapability</span><span class="sxs-lookup"><span data-stu-id="fffa2-103">meetingCapability resource type</span></span>

> <span data-ttu-id="fffa2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fffa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fffa2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fffa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fffa2-106">Enthält die Funktionen einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="fffa2-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="fffa2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fffa2-107">Properties</span></span>

| <span data-ttu-id="fffa2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fffa2-108">Property</span></span>                          | <span data-ttu-id="fffa2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fffa2-109">Type</span></span>    | <span data-ttu-id="fffa2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fffa2-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="fffa2-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="fffa2-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="fffa2-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fffa2-112">Boolean</span></span> | <span data-ttu-id="fffa2-113">Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="fffa2-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="fffa2-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="fffa2-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="fffa2-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fffa2-115">Boolean</span></span> | <span data-ttu-id="fffa2-116">Gibt an, ob anonyme Benutzer zugelassen sind, um eine Besprechung zu starten.</span><span class="sxs-lookup"><span data-stu-id="fffa2-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="fffa2-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="fffa2-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="fffa2-118">String</span><span class="sxs-lookup"><span data-stu-id="fffa2-118">String</span></span>  | <span data-ttu-id="fffa2-119">Mögliche Werte: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="fffa2-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="fffa2-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fffa2-120">JSON representation</span></span>

<span data-ttu-id="fffa2-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fffa2-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
