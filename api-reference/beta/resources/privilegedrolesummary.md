---
title: Ressourcentyp privilegedRoleSummary
description: Die Statistiken für eine bestimmte Rolle Zusammenfassung.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513739"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="71cf3-103">Ressourcentyp privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="71cf3-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71cf3-104">Die Statistiken für eine bestimmte Rolle Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="71cf3-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="71cf3-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="71cf3-105">Methods</span></span>

| <span data-ttu-id="71cf3-106">Methode</span><span class="sxs-lookup"><span data-stu-id="71cf3-106">Method</span></span>           | <span data-ttu-id="71cf3-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="71cf3-107">Return Type</span></span>    |<span data-ttu-id="71cf3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71cf3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71cf3-109">Abrufen von privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="71cf3-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="71cf3-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="71cf3-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="71cf3-111">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71cf3-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71cf3-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71cf3-112">Properties</span></span>
| <span data-ttu-id="71cf3-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71cf3-113">Property</span></span>     | <span data-ttu-id="71cf3-114">Typ</span><span class="sxs-lookup"><span data-stu-id="71cf3-114">Type</span></span>   |<span data-ttu-id="71cf3-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71cf3-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71cf3-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="71cf3-116">elevatedCount</span></span>|<span data-ttu-id="71cf3-117">int32</span><span class="sxs-lookup"><span data-stu-id="71cf3-117">int32</span></span>|<span data-ttu-id="71cf3-118">Die Anzahl der Benutzer, die die Rolle zugewiesen haben, ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="71cf3-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="71cf3-119">id</span><span class="sxs-lookup"><span data-stu-id="71cf3-119">id</span></span>|<span data-ttu-id="71cf3-120">string</span><span class="sxs-lookup"><span data-stu-id="71cf3-120">string</span></span>| <span data-ttu-id="71cf3-121">Der eindeutige Bezeichner für die Rolle.</span><span class="sxs-lookup"><span data-stu-id="71cf3-121">The unique identifier for the role.</span></span> <span data-ttu-id="71cf3-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71cf3-122">Read-only.</span></span>|
|<span data-ttu-id="71cf3-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="71cf3-123">managedCount</span></span>|<span data-ttu-id="71cf3-124">int32</span><span class="sxs-lookup"><span data-stu-id="71cf3-124">int32</span></span>|<span data-ttu-id="71cf3-125">Die Anzahl der Benutzer, die die Rolle zugewiesen haben, aber die Rolle ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="71cf3-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="71cf3-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="71cf3-126">mfaEnabled</span></span>|<span data-ttu-id="71cf3-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71cf3-127">boolean</span></span>|<span data-ttu-id="71cf3-128">**true,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="71cf3-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="71cf3-129">**false,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="71cf3-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="71cf3-130">status</span><span class="sxs-lookup"><span data-stu-id="71cf3-130">status</span></span>|<span data-ttu-id="71cf3-131">string</span><span class="sxs-lookup"><span data-stu-id="71cf3-131">string</span></span>| <span data-ttu-id="71cf3-132">Mögliche Werte sind: `ok` und `bad`.</span><span class="sxs-lookup"><span data-stu-id="71cf3-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="71cf3-133">Der Wert hängt das Verhältnis von (ManagedCount / UsersCount).</span><span class="sxs-lookup"><span data-stu-id="71cf3-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="71cf3-134">Wenn das Verhältnis einen vordefinierten Schwellenwert unterschreitet `ok` wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71cf3-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="71cf3-135">Andernfalls `bad` wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71cf3-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="71cf3-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="71cf3-136">usersCount</span></span>|<span data-ttu-id="71cf3-137">int32</span><span class="sxs-lookup"><span data-stu-id="71cf3-137">int32</span></span>|<span data-ttu-id="71cf3-138">Die Anzahl der Benutzer, die mit der Rolle zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="71cf3-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71cf3-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71cf3-139">Relationships</span></span>
<span data-ttu-id="71cf3-140">Keine</span><span class="sxs-lookup"><span data-stu-id="71cf3-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="71cf3-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71cf3-141">JSON representation</span></span>

<span data-ttu-id="71cf3-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71cf3-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
