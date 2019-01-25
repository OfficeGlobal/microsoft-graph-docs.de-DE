---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524289"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="c5c11-103">Ressourcentyp meetingCapability</span><span class="sxs-lookup"><span data-stu-id="c5c11-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c11-104">Enthält die Funktionen einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="c5c11-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="c5c11-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5c11-105">Properties</span></span>

| <span data-ttu-id="c5c11-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5c11-106">Property</span></span>                          | <span data-ttu-id="c5c11-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c5c11-107">Type</span></span>    | <span data-ttu-id="c5c11-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5c11-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="c5c11-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="c5c11-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="c5c11-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5c11-110">Boolean</span></span> | <span data-ttu-id="c5c11-111">Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c5c11-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="c5c11-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="c5c11-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="c5c11-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c5c11-113">Boolean</span></span> | <span data-ttu-id="c5c11-114">Gibt an, ob anonyme Benutzer zugelassen sind, um eine Besprechung zu starten.</span><span class="sxs-lookup"><span data-stu-id="c5c11-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="c5c11-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="c5c11-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="c5c11-116">String</span><span class="sxs-lookup"><span data-stu-id="c5c11-116">String</span></span>  | <span data-ttu-id="c5c11-117">Mögliche Werte: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="c5c11-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="c5c11-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5c11-118">JSON representation</span></span>

<span data-ttu-id="c5c11-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c5c11-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
