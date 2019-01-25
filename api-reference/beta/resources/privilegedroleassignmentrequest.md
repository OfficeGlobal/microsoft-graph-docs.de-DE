---
title: Ressourcentyp privilegedRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509007"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="de967-103">Ressourcentyp privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="de967-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de967-104">Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="de967-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="de967-105">`privilegedRoleAssignmentRequest`wird eine Entität Ticket modelliert verwaltet den Lebenszyklus von rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="de967-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="de967-106">Es stellt die Absicht/Entscheidung von Benutzern und Administratoren und bietet außerdem die Flexibilität zum Aktivieren der Implementierung von wiederkehrenden Schduling, Gates Genehmigung und usw., im Vergleich zu direkt Verfügbarmachen `POST` und `LIST` Vorgänge sowie `MY` und `Cancel` -Funktionen auf `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="de967-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="de967-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="de967-107">Methods</span></span>

| <span data-ttu-id="de967-108">Methode</span><span class="sxs-lookup"><span data-stu-id="de967-108">Method</span></span>       | <span data-ttu-id="de967-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="de967-109">Return Type</span></span> | <span data-ttu-id="de967-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de967-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="de967-111">List</span><span class="sxs-lookup"><span data-stu-id="de967-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="de967-112">[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="de967-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="de967-113">Role Assignment Anforderungen aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="de967-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="de967-114">Create</span><span class="sxs-lookup"><span data-stu-id="de967-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="de967-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="de967-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="de967-116">Erstellen Sie eine Anforderung an den Lebenszyklus von vorhandenen oder neuen rollenzuweisung zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="de967-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="de967-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="de967-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="de967-118">Ausstehende Role Assignment Anforderung abbrechen.</span><span class="sxs-lookup"><span data-stu-id="de967-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="de967-119">My</span><span class="sxs-lookup"><span data-stu-id="de967-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="de967-120">GET-Anforderung für Rolle-Zuordnung für aktuellen Requstor.</span><span class="sxs-lookup"><span data-stu-id="de967-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="de967-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de967-121">Properties</span></span>

| <span data-ttu-id="de967-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de967-122">Property</span></span>     | <span data-ttu-id="de967-123">Typ</span><span class="sxs-lookup"><span data-stu-id="de967-123">Type</span></span>        | <span data-ttu-id="de967-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de967-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de967-125">id</span><span class="sxs-lookup"><span data-stu-id="de967-125">id</span></span>|<span data-ttu-id="de967-126">String</span><span class="sxs-lookup"><span data-stu-id="de967-126">String</span></span>| <span data-ttu-id="de967-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="de967-127">Read-only.</span></span> <span data-ttu-id="de967-128">Die Id der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de967-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="de967-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de967-129">assignmentState</span></span>|<span data-ttu-id="de967-130">String</span><span class="sxs-lookup"><span data-stu-id="de967-130">String</span></span>| <span data-ttu-id="de967-131">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="de967-131">The state of the assignment.</span></span> <span data-ttu-id="de967-132">Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="de967-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="de967-133">duration</span><span class="sxs-lookup"><span data-stu-id="de967-133">duration</span></span>|<span data-ttu-id="de967-134">String</span><span class="sxs-lookup"><span data-stu-id="de967-134">String</span></span>| <span data-ttu-id="de967-135">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="de967-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="de967-136">Grund</span><span class="sxs-lookup"><span data-stu-id="de967-136">reason</span></span>|<span data-ttu-id="de967-137">String</span><span class="sxs-lookup"><span data-stu-id="de967-137">String</span></span>| <span data-ttu-id="de967-138">Der Grund für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="de967-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="de967-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="de967-139">requestedDateTime</span></span>|<span data-ttu-id="de967-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de967-140">DateTimeOffset</span></span>| <span data-ttu-id="de967-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="de967-141">Read-only.</span></span> <span data-ttu-id="de967-142">Die Zeit zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="de967-142">The request create time.</span></span> <span data-ttu-id="de967-143">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="de967-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de967-144">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="de967-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="de967-145">roleId</span><span class="sxs-lookup"><span data-stu-id="de967-145">roleId</span></span>|<span data-ttu-id="de967-146">String</span><span class="sxs-lookup"><span data-stu-id="de967-146">String</span></span>| <span data-ttu-id="de967-147">Die Id der Rolle.</span><span class="sxs-lookup"><span data-stu-id="de967-147">The id of the role.</span></span>|
|<span data-ttu-id="de967-148">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="de967-148">schedule</span></span>|[<span data-ttu-id="de967-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de967-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="de967-150">Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.</span><span class="sxs-lookup"><span data-stu-id="de967-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="de967-151">status</span><span class="sxs-lookup"><span data-stu-id="de967-151">status</span></span>|<span data-ttu-id="de967-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de967-152">String</span></span>| <span data-ttu-id="de967-153">Lesen vorbehalten Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="de967-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="de967-154">Der Wert kann sein `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="de967-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="de967-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="de967-155">ticketNumber</span></span>|<span data-ttu-id="de967-156">String</span><span class="sxs-lookup"><span data-stu-id="de967-156">String</span></span>| <span data-ttu-id="de967-157">Die TicketNumber für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="de967-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="de967-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="de967-158">ticketSystem</span></span>|<span data-ttu-id="de967-159">String</span><span class="sxs-lookup"><span data-stu-id="de967-159">String</span></span>| <span data-ttu-id="de967-160">Die TicketSystem für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="de967-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="de967-161">type</span><span class="sxs-lookup"><span data-stu-id="de967-161">type</span></span>|<span data-ttu-id="de967-162">String</span><span class="sxs-lookup"><span data-stu-id="de967-162">String</span></span>| <span data-ttu-id="de967-163">Darstellen der den Typ des Vorgangs für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="de967-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="de967-164">Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="de967-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="de967-165">userId</span><span class="sxs-lookup"><span data-stu-id="de967-165">userId</span></span>|<span data-ttu-id="de967-166">String</span><span class="sxs-lookup"><span data-stu-id="de967-166">String</span></span>| <span data-ttu-id="de967-167">Die Id des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="de967-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de967-168">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="de967-168">Relationships</span></span>
| <span data-ttu-id="de967-169">Beziehung</span><span class="sxs-lookup"><span data-stu-id="de967-169">Relationship</span></span> | <span data-ttu-id="de967-170">Typ</span><span class="sxs-lookup"><span data-stu-id="de967-170">Type</span></span>        | <span data-ttu-id="de967-171">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de967-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de967-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="de967-172">roleInfo</span></span>|[<span data-ttu-id="de967-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="de967-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="de967-174">Das Objekt RoleInfo der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de967-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de967-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de967-175">JSON representation</span></span>

<span data-ttu-id="de967-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de967-176">The following is a JSON representation of the resource.</span></span>

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
