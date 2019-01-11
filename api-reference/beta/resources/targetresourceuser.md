---
title: Ressourcentyp targetResourceUser
description: Gibt das Benutzerobjekt, das hinzugefügt wurde, aktualisiert oder gelöscht von Administratoren als Teil des Audit-Aktivität an. Die Ressource TargetResource abgeleitet.
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831928"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="bc30b-104">Ressourcentyp targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="bc30b-104">targetResourceUser resource type</span></span>
<span data-ttu-id="bc30b-105">Gibt das Benutzerobjekt, das hinzugefügt wurde, aktualisiert oder gelöscht von Administratoren als Teil des Audit-Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="bc30b-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="bc30b-106">Die Ressource [TargetResource](targetresource.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="bc30b-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="bc30b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc30b-107">Properties</span></span>
| <span data-ttu-id="bc30b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc30b-108">Property</span></span>     | <span data-ttu-id="bc30b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bc30b-109">Type</span></span>   |<span data-ttu-id="bc30b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc30b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc30b-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc30b-111">userPrincipalName</span></span>|<span data-ttu-id="bc30b-112">String</span><span class="sxs-lookup"><span data-stu-id="bc30b-112">String</span></span>|<span data-ttu-id="bc30b-113">Gibt die eindeutige Id des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="bc30b-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="bc30b-114">Verweist auf die Benutzer-Id für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="bc30b-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc30b-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc30b-115">JSON representation</span></span>

<span data-ttu-id="bc30b-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc30b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
