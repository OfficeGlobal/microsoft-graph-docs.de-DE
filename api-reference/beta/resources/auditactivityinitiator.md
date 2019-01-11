---
title: Ressourcentyp auditActivityInitiator
description: Identität das Resource-Objekt, das die Aktivität initiiert. Der Initiator kann es sich um einen Benutzer, eine app oder eines Systems (die als eine app betrachtet wird)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884609"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="62554-104">Ressourcentyp auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="62554-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="62554-105">Identität das Resource-Objekt, das die Aktivität initiiert.</span><span class="sxs-lookup"><span data-stu-id="62554-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="62554-106">Der Initiator kann es sich um einen Benutzer, eine app oder eines Systems (die als eine app betrachtet wird)</span><span class="sxs-lookup"><span data-stu-id="62554-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="62554-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="62554-107">Properties</span></span>
| <span data-ttu-id="62554-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62554-108">Property</span></span>     | <span data-ttu-id="62554-109">Typ</span><span class="sxs-lookup"><span data-stu-id="62554-109">Type</span></span>   |<span data-ttu-id="62554-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62554-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62554-111">App</span><span class="sxs-lookup"><span data-stu-id="62554-111">app</span></span>|[<span data-ttu-id="62554-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="62554-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="62554-113">Wenn die Ressource die Aktivität Initiieren einer app ist, gibt diese Eigenschaft alle app weiterführende Informationen wie AppId, Name, ServicePrincipalId Name.</span><span class="sxs-lookup"><span data-stu-id="62554-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="62554-114">user</span><span class="sxs-lookup"><span data-stu-id="62554-114">user</span></span>|[<span data-ttu-id="62554-115">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="62554-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="62554-116">Wenn die Ressource die Aktivität Initiieren eines Benutzers ist, gibt diese Eigenschaft alle Benutzer weiterführende Informationen wie Benutzer-ID, Name, userPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="62554-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62554-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="62554-117">JSON representation</span></span>

<span data-ttu-id="62554-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="62554-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
