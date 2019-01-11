---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 3a7f291c81522d33bffbcce6e97a407f09234db5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825809"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="b517a-103">Ressourcentyp meetingCapability</span><span class="sxs-lookup"><span data-stu-id="b517a-103">meetingCapability resource type</span></span>

> <span data-ttu-id="b517a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b517a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b517a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b517a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b517a-106">Enthält die Funktionen einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="b517a-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="b517a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b517a-107">Properties</span></span>

| <span data-ttu-id="b517a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b517a-108">Property</span></span>                          | <span data-ttu-id="b517a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b517a-109">Type</span></span>    | <span data-ttu-id="b517a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b517a-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="b517a-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="b517a-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="b517a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b517a-112">Boolean</span></span> | <span data-ttu-id="b517a-113">Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b517a-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="b517a-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="b517a-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="b517a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b517a-115">Boolean</span></span> | <span data-ttu-id="b517a-116">Gibt an, ob anonyme Benutzer zugelassen sind, um eine Besprechung zu starten.</span><span class="sxs-lookup"><span data-stu-id="b517a-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="b517a-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="b517a-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="b517a-118">String</span><span class="sxs-lookup"><span data-stu-id="b517a-118">String</span></span>  | <span data-ttu-id="b517a-119">Mögliche Werte: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="b517a-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="b517a-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b517a-120">JSON representation</span></span>

<span data-ttu-id="b517a-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b517a-121">The following is a JSON representation of the resource.</span></span>

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
