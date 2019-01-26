---
title: Ressourcentyp privilegedRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
localization_priority: Normal
ms.openlocfilehash: a0cb0bc03d8bb2436e45139bc9db5322cc3970cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571748"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="68c34-103">Ressourcentyp privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="68c34-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68c34-104">Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="68c34-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="68c34-105">`privilegedRoleAssignmentRequest`wird eine Entität Ticket modelliert verwaltet den Lebenszyklus von rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="68c34-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="68c34-106">Es stellt die Absicht/Entscheidung von Benutzern und Administratoren und bietet außerdem die Flexibilität zum Aktivieren der Implementierung von wiederkehrenden Schduling, Gates Genehmigung und usw., im Vergleich zu direkt Verfügbarmachen `POST` und `LIST` Vorgänge sowie `MY` und `Cancel` -Funktionen auf `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="68c34-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="68c34-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="68c34-107">Methods</span></span>

| <span data-ttu-id="68c34-108">Methode</span><span class="sxs-lookup"><span data-stu-id="68c34-108">Method</span></span>       | <span data-ttu-id="68c34-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="68c34-109">Return Type</span></span> | <span data-ttu-id="68c34-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68c34-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="68c34-111">List</span><span class="sxs-lookup"><span data-stu-id="68c34-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="68c34-112">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="68c34-112">[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="68c34-113">Role Assignment Anforderungen aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="68c34-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="68c34-114">Create</span><span class="sxs-lookup"><span data-stu-id="68c34-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="68c34-115">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="68c34-115">privilegedRoleAssignmentRequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="68c34-116">Erstellen Sie eine Anforderung an den Lebenszyklus von vorhandenen oder neuen rollenzuweisung zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="68c34-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="68c34-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="68c34-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="68c34-118">Ausstehende Role Assignment Anforderung abbrechen.</span><span class="sxs-lookup"><span data-stu-id="68c34-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="68c34-119">My</span><span class="sxs-lookup"><span data-stu-id="68c34-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="68c34-120">GET-Anforderung für Rolle-Zuordnung für aktuellen Requestor.</span><span class="sxs-lookup"><span data-stu-id="68c34-120">Get role assignment request for current requestor.</span></span>|

## <a name="properties"></a><span data-ttu-id="68c34-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68c34-121">Properties</span></span>

| <span data-ttu-id="68c34-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68c34-122">Property</span></span>     | <span data-ttu-id="68c34-123">Typ</span><span class="sxs-lookup"><span data-stu-id="68c34-123">Type</span></span>        | <span data-ttu-id="68c34-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68c34-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68c34-125">id</span><span class="sxs-lookup"><span data-stu-id="68c34-125">id</span></span>|<span data-ttu-id="68c34-126">String</span><span class="sxs-lookup"><span data-stu-id="68c34-126">String</span></span>| <span data-ttu-id="68c34-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="68c34-127">Read-only.</span></span> <span data-ttu-id="68c34-128">Die Id der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68c34-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="68c34-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="68c34-129">assignmentState</span></span>|<span data-ttu-id="68c34-130">String</span><span class="sxs-lookup"><span data-stu-id="68c34-130">String</span></span>| <span data-ttu-id="68c34-131">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="68c34-131">The state of the assignment.</span></span> <span data-ttu-id="68c34-132">Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="68c34-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="68c34-133">duration</span><span class="sxs-lookup"><span data-stu-id="68c34-133">duration</span></span>|<span data-ttu-id="68c34-134">String</span><span class="sxs-lookup"><span data-stu-id="68c34-134">String</span></span>| <span data-ttu-id="68c34-135">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="68c34-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="68c34-136">Grund</span><span class="sxs-lookup"><span data-stu-id="68c34-136">reason</span></span>|<span data-ttu-id="68c34-137">String</span><span class="sxs-lookup"><span data-stu-id="68c34-137">String</span></span>| <span data-ttu-id="68c34-138">Der Grund für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="68c34-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="68c34-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="68c34-139">requestedDateTime</span></span>|<span data-ttu-id="68c34-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c34-140">DateTimeOffset</span></span>| <span data-ttu-id="68c34-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="68c34-141">Read-only.</span></span> <span data-ttu-id="68c34-142">Die Zeit zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="68c34-142">The request create time.</span></span> <span data-ttu-id="68c34-143">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="68c34-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68c34-144">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="68c34-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="68c34-145">roleId</span><span class="sxs-lookup"><span data-stu-id="68c34-145">roleId</span></span>|<span data-ttu-id="68c34-146">String</span><span class="sxs-lookup"><span data-stu-id="68c34-146">String</span></span>| <span data-ttu-id="68c34-147">Die Id der Rolle.</span><span class="sxs-lookup"><span data-stu-id="68c34-147">The id of the role.</span></span>|
|<span data-ttu-id="68c34-148">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="68c34-148">schedule</span></span>|[<span data-ttu-id="68c34-149">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="68c34-149"> microsoft.graph.governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="68c34-150">Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.</span><span class="sxs-lookup"><span data-stu-id="68c34-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="68c34-151">status</span><span class="sxs-lookup"><span data-stu-id="68c34-151">status</span></span>|<span data-ttu-id="68c34-152">String</span><span class="sxs-lookup"><span data-stu-id="68c34-152">String</span></span>| <span data-ttu-id="68c34-153">Lesen vorbehalten Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="68c34-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="68c34-154">Der Wert kann sein `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="68c34-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="68c34-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="68c34-155">ticketNumber</span></span>|<span data-ttu-id="68c34-156">String</span><span class="sxs-lookup"><span data-stu-id="68c34-156">String</span></span>| <span data-ttu-id="68c34-157">Die TicketNumber für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="68c34-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="68c34-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="68c34-158">ticketSystem</span></span>|<span data-ttu-id="68c34-159">String</span><span class="sxs-lookup"><span data-stu-id="68c34-159">String</span></span>| <span data-ttu-id="68c34-160">Die TicketSystem für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="68c34-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="68c34-161">type</span><span class="sxs-lookup"><span data-stu-id="68c34-161">type</span></span>|<span data-ttu-id="68c34-162">String</span><span class="sxs-lookup"><span data-stu-id="68c34-162">String</span></span>| <span data-ttu-id="68c34-163">Darstellen der den Typ des Vorgangs für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="68c34-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="68c34-164">Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="68c34-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="68c34-165">userId</span><span class="sxs-lookup"><span data-stu-id="68c34-165">userId</span></span>|<span data-ttu-id="68c34-166">String</span><span class="sxs-lookup"><span data-stu-id="68c34-166">String</span></span>| <span data-ttu-id="68c34-167">Die Id des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="68c34-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68c34-168">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68c34-168">Relationships</span></span>
| <span data-ttu-id="68c34-169">Beziehung</span><span class="sxs-lookup"><span data-stu-id="68c34-169">Relationship</span></span> | <span data-ttu-id="68c34-170">Typ</span><span class="sxs-lookup"><span data-stu-id="68c34-170">Type</span></span>        | <span data-ttu-id="68c34-171">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68c34-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68c34-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="68c34-172">roleInfo</span></span>|[<span data-ttu-id="68c34-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="68c34-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="68c34-174">Das Objekt RoleInfo der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68c34-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68c34-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68c34-175">JSON representation</span></span>

<span data-ttu-id="68c34-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68c34-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
