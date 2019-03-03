---
title: securityActionState-Ressourcentyp
description: Stellt den Verlauf der Änderungen des SecurityAction-Zustands dar.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366931"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="46950-103">securityActionState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46950-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46950-104">Stellt den Verlauf der Änderungen des SecurityAction-Zustands dar.</span><span class="sxs-lookup"><span data-stu-id="46950-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="46950-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46950-105">Properties</span></span>

| <span data-ttu-id="46950-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46950-106">Property</span></span>     | <span data-ttu-id="46950-107">Typ</span><span class="sxs-lookup"><span data-stu-id="46950-107">Type</span></span>        | <span data-ttu-id="46950-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46950-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46950-109">appId</span><span class="sxs-lookup"><span data-stu-id="46950-109">appId</span></span>|<span data-ttu-id="46950-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46950-110">String</span></span>|<span data-ttu-id="46950-111">Die Anwendungs-ID der aufrufenden Anwendung, die ein Update (PATCH) an die Aktion gesendet hat.</span><span class="sxs-lookup"><span data-stu-id="46950-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="46950-112">Der `appId` sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="46950-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="46950-113">status</span><span class="sxs-lookup"><span data-stu-id="46950-113">status</span></span>|<span data-ttu-id="46950-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46950-114">String</span></span>| <span data-ttu-id="46950-115">Status der SecurityAction in diesem Update.</span><span class="sxs-lookup"><span data-stu-id="46950-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="46950-116">Mögliche Werte: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="46950-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="46950-117">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="46950-117">updatedDateTime</span></span>|<span data-ttu-id="46950-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46950-118">DateTimeOffset</span></span>| <span data-ttu-id="46950-119">Timestamp, als der Actionstate wurden aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="46950-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="46950-120">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="46950-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46950-121">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46950-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46950-122">user</span><span class="sxs-lookup"><span data-stu-id="46950-122">user</span></span>|<span data-ttu-id="46950-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46950-123">String</span></span>|<span data-ttu-id="46950-124">Der Benutzerprinzipalname des angemeldeten Benutzers, der ein Update (PATCH) an die Aktion gesendet hat.</span><span class="sxs-lookup"><span data-stu-id="46950-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="46950-125">Der `user` sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="46950-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46950-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46950-126">JSON representation</span></span>

<span data-ttu-id="46950-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46950-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
