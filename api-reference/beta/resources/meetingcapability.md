---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061416"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="5ea0b-103">Ressourcentyp meetingCapability</span><span class="sxs-lookup"><span data-stu-id="5ea0b-103">meetingCapability resource type</span></span>

> <span data-ttu-id="5ea0b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5ea0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ea0b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ea0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ea0b-106">Enthält die Funktionen einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="5ea0b-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="5ea0b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5ea0b-107">Properties</span></span>

| <span data-ttu-id="5ea0b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ea0b-108">Property</span></span>       | <span data-ttu-id="5ea0b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5ea0b-109">Type</span></span>    | <span data-ttu-id="5ea0b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ea0b-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ea0b-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="5ea0b-111">allowAnonymousUsersToDialOut</span></span> | <span data-ttu-id="5ea0b-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5ea0b-112">Boolean</span></span> | <span data-ttu-id="5ea0b-113">Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="5ea0b-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="5ea0b-114">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="5ea0b-114">autoAdmittedUsers</span></span> | <span data-ttu-id="5ea0b-115">String</span><span class="sxs-lookup"><span data-stu-id="5ea0b-115">String</span></span> | <span data-ttu-id="5ea0b-116">Mögliche Werte: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="5ea0b-116">Possible values are: `everyoneInCompany`, `everyone`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ea0b-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5ea0b-117">JSON representation</span></span>

<span data-ttu-id="5ea0b-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5ea0b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
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
