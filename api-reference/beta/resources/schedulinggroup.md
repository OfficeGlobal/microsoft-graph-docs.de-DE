---
title: schedulingGroup-Ressourcentyp
description: Eine logische Gruppierung von Mitgliedern im Zeitplan (in der Regel anhand der Rolle).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657868"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="fd781-103">schedulingGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd781-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd781-104">Eine logische Gruppierung von Benutzern in einem [Zeitplan](schedule.md) (in der Regel anhand der Rolle).</span><span class="sxs-lookup"><span data-stu-id="fd781-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="fd781-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="fd781-105">Methods</span></span>

| <span data-ttu-id="fd781-106">Methode</span><span class="sxs-lookup"><span data-stu-id="fd781-106">Method</span></span>       | <span data-ttu-id="fd781-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fd781-107">Return Type</span></span>  |<span data-ttu-id="fd781-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd781-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd781-109">schedulingGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="fd781-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="fd781-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fd781-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fd781-111">Ein neues `schedulingGroup` erstellen.</span><span class="sxs-lookup"><span data-stu-id="fd781-111">`schedulingGroup`</span></span>|
|[<span data-ttu-id="fd781-112">schedulingGroup auflisten</span><span class="sxs-lookup"><span data-stu-id="fd781-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="fd781-113">[schedulingGroup](schedulinggroup.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="fd781-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="fd781-114">Abrufen der Liste von `schedulingGroups` in einem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="fd781-114">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="fd781-115">schedulingGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="fd781-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="fd781-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fd781-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fd781-117">Abrufen eines `schedulingGroup` anhand der ID.</span><span class="sxs-lookup"><span data-stu-id="fd781-117">Get a drive by ID</span></span>|
|[<span data-ttu-id="fd781-118">schedulingGroup ersetzen</span><span class="sxs-lookup"><span data-stu-id="fd781-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="fd781-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fd781-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="fd781-120">Ein `schedulingGroup` ersetzen.</span><span class="sxs-lookup"><span data-stu-id="fd781-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="fd781-121">schedulingGroup löschen</span><span class="sxs-lookup"><span data-stu-id="fd781-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="fd781-122">Keine</span><span class="sxs-lookup"><span data-stu-id="fd781-122">None</span></span> | <span data-ttu-id="fd781-123">`schedulingGroup` als inaktiv markieren.</span><span class="sxs-lookup"><span data-stu-id="fd781-123">Mark an Account as inactive</span></span>|

## <a name="properties"></a><span data-ttu-id="fd781-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd781-124">Properties</span></span>
|<span data-ttu-id="fd781-125">Name</span><span class="sxs-lookup"><span data-stu-id="fd781-125">Name</span></span>          |<span data-ttu-id="fd781-126">Typ</span><span class="sxs-lookup"><span data-stu-id="fd781-126">Type</span></span>           |<span data-ttu-id="fd781-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd781-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="fd781-128">id</span><span class="sxs-lookup"><span data-stu-id="fd781-128">id</span></span>            | `string`      |<span data-ttu-id="fd781-129">ID des `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fd781-129">`schedulingGroup` - ID of the Teacher</span></span>|
| <span data-ttu-id="fd781-130">displayName</span><span class="sxs-lookup"><span data-stu-id="fd781-130">displayName</span></span>   | `string`      | <span data-ttu-id="fd781-131">Der Anzeigename für das `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="fd781-131">The display name of the user.</span></span> <span data-ttu-id="fd781-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd781-132">Required.</span></span> |
| <span data-ttu-id="fd781-133">isActive</span><span class="sxs-lookup"><span data-stu-id="fd781-133">isActive</span></span>          |`bool`      | <span data-ttu-id="fd781-134">Gibt an, ob `schedulingGroup` beim Erstellen neuer Entitäten oder beim Aktualisieren vorhandener Entitäten verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="fd781-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="fd781-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd781-135">Required.</span></span> |
| <span data-ttu-id="fd781-136">UserIds</span><span class="sxs-lookup"><span data-stu-id="fd781-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="fd781-137">Die Liste der Benutzer-IDs, die ein Mitglied von `schedulingGroup` sind.</span><span class="sxs-lookup"><span data-stu-id="fd781-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="fd781-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd781-138">Required.</span></span> |
| <span data-ttu-id="fd781-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd781-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="fd781-140">Der Zeitstempel, mit dem dieses `schedulingGroup` zuerst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="fd781-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="fd781-141">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="fd781-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd781-142">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="fd781-142">For example, midnight UTC on Jan 1, 2014 would look like this: .</span></span> |
| <span data-ttu-id="fd781-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd781-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="fd781-144">Der Zeitstempel, mit dem dieses `schedulingGroup` zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="fd781-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="fd781-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="fd781-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd781-146">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="fd781-146">For example, midnight UTC on Jan 1, 2014 would look like this: .</span></span> |
| <span data-ttu-id="fd781-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fd781-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="fd781-148">Die Identität, die dieses `schedulingGroup` zuletzt aktualisiert hat.</span><span class="sxs-lookup"><span data-stu-id="fd781-148">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd781-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd781-149">JSON representation</span></span>

<span data-ttu-id="fd781-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd781-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
