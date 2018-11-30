---
title: Ressourcentyp privilegedRoleSummary
description: Die Statistiken für eine bestimmte Rolle Zusammenfassung.
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064652"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="2b790-103">Ressourcentyp privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2b790-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="2b790-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b790-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b790-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b790-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b790-106">Die Statistiken für eine bestimmte Rolle Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="2b790-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="2b790-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="2b790-107">Methods</span></span>

| <span data-ttu-id="2b790-108">Methode</span><span class="sxs-lookup"><span data-stu-id="2b790-108">Method</span></span>           | <span data-ttu-id="2b790-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2b790-109">Return Type</span></span>    |<span data-ttu-id="2b790-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b790-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b790-111">Abrufen von privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2b790-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="2b790-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2b790-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="2b790-113">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b790-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b790-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2b790-114">Properties</span></span>
| <span data-ttu-id="2b790-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b790-115">Property</span></span>     | <span data-ttu-id="2b790-116">Typ</span><span class="sxs-lookup"><span data-stu-id="2b790-116">Type</span></span>   |<span data-ttu-id="2b790-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b790-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b790-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="2b790-118">elevatedCount</span></span>|<span data-ttu-id="2b790-119">int32</span><span class="sxs-lookup"><span data-stu-id="2b790-119">int32</span></span>|<span data-ttu-id="2b790-120">Die Anzahl der Benutzer, die die Rolle zugewiesen haben, ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2b790-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="2b790-121">id</span><span class="sxs-lookup"><span data-stu-id="2b790-121">id</span></span>|<span data-ttu-id="2b790-122">string</span><span class="sxs-lookup"><span data-stu-id="2b790-122">string</span></span>| <span data-ttu-id="2b790-123">Der eindeutige Bezeichner für die Rolle.</span><span class="sxs-lookup"><span data-stu-id="2b790-123">The unique identifier for the role.</span></span> <span data-ttu-id="2b790-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2b790-124">Read-only.</span></span>|
|<span data-ttu-id="2b790-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="2b790-125">managedCount</span></span>|<span data-ttu-id="2b790-126">int32</span><span class="sxs-lookup"><span data-stu-id="2b790-126">int32</span></span>|<span data-ttu-id="2b790-127">Die Anzahl der Benutzer, die die Rolle zugewiesen haben, aber die Rolle ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="2b790-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="2b790-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="2b790-128">mfaEnabled</span></span>|<span data-ttu-id="2b790-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b790-129">boolean</span></span>|<span data-ttu-id="2b790-130">**true,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2b790-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="2b790-131">**false,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2b790-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="2b790-132">status</span><span class="sxs-lookup"><span data-stu-id="2b790-132">status</span></span>|<span data-ttu-id="2b790-133">string</span><span class="sxs-lookup"><span data-stu-id="2b790-133">string</span></span>| <span data-ttu-id="2b790-134">Mögliche Werte sind: `ok` und `bad`.</span><span class="sxs-lookup"><span data-stu-id="2b790-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="2b790-135">Der Wert hängt das Verhältnis von (ManagedCount / UsersCount).</span><span class="sxs-lookup"><span data-stu-id="2b790-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="2b790-136">Wenn das Verhältnis einen vordefinierten Schwellenwert unterschreitet `ok` wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b790-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="2b790-137">Andernfalls `bad` wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b790-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="2b790-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="2b790-138">usersCount</span></span>|<span data-ttu-id="2b790-139">int32</span><span class="sxs-lookup"><span data-stu-id="2b790-139">int32</span></span>|<span data-ttu-id="2b790-140">Die Anzahl der Benutzer, die mit der Rolle zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="2b790-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b790-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2b790-141">Relationships</span></span>
<span data-ttu-id="2b790-142">Keine</span><span class="sxs-lookup"><span data-stu-id="2b790-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b790-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2b790-143">JSON representation</span></span>

<span data-ttu-id="2b790-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2b790-144">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->