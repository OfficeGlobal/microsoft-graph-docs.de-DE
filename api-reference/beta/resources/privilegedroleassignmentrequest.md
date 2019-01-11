---
title: Ressourcentyp privilegedRoleAssignmentRequest
description: Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.
localization_priority: Normal
ms.openlocfilehash: bfe3b6802136b2848f36abef08134efd0eb82518
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880129"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="28dcf-103">Ressourcentyp privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="28dcf-103">privilegedRoleAssignmentRequest resource type</span></span>

> <span data-ttu-id="28dcf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="28dcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28dcf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28dcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28dcf-106">Stellt die Anforderung für Role Assignment Vorgänge in Privilegd Identity Management.</span><span class="sxs-lookup"><span data-stu-id="28dcf-106">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="28dcf-107">`privilegedRoleAssignmentRequest`wird eine Entität Ticket modelliert verwaltet den Lebenszyklus von rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="28dcf-107">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="28dcf-108">Es stellt die Absicht/Entscheidung von Benutzern und Administratoren und bietet außerdem die Flexibilität zum Aktivieren der Implementierung von wiederkehrenden Schduling, Gates Genehmigung und usw., im Vergleich zu direkt Verfügbarmachen `POST` und `LIST` Vorgänge sowie `MY` und `Cancel` -Funktionen auf `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="28dcf-108">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="28dcf-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="28dcf-109">Methods</span></span>

| <span data-ttu-id="28dcf-110">Methode</span><span class="sxs-lookup"><span data-stu-id="28dcf-110">Method</span></span>       | <span data-ttu-id="28dcf-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="28dcf-111">Return Type</span></span> | <span data-ttu-id="28dcf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28dcf-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="28dcf-113">List</span><span class="sxs-lookup"><span data-stu-id="28dcf-113">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="28dcf-114">[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="28dcf-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="28dcf-115">Role Assignment Anforderungen aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="28dcf-115">List role assignment requests.</span></span>|
|[<span data-ttu-id="28dcf-116">Create</span><span class="sxs-lookup"><span data-stu-id="28dcf-116">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="28dcf-117">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="28dcf-117">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="28dcf-118">Erstellen Sie eine Anforderung an den Lebenszyklus von vorhandenen oder neuen rollenzuweisung zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="28dcf-118">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="28dcf-119">Abbrechen</span><span class="sxs-lookup"><span data-stu-id="28dcf-119">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="28dcf-120">Ausstehende Role Assignment Anforderung abbrechen.</span><span class="sxs-lookup"><span data-stu-id="28dcf-120">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="28dcf-121">My</span><span class="sxs-lookup"><span data-stu-id="28dcf-121">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="28dcf-122">GET-Anforderung für Rolle-Zuordnung für aktuellen Requstor.</span><span class="sxs-lookup"><span data-stu-id="28dcf-122">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="28dcf-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28dcf-123">Properties</span></span>

| <span data-ttu-id="28dcf-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28dcf-124">Property</span></span>     | <span data-ttu-id="28dcf-125">Typ</span><span class="sxs-lookup"><span data-stu-id="28dcf-125">Type</span></span>        | <span data-ttu-id="28dcf-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28dcf-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28dcf-127">id</span><span class="sxs-lookup"><span data-stu-id="28dcf-127">id</span></span>|<span data-ttu-id="28dcf-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-128">String</span></span>| <span data-ttu-id="28dcf-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="28dcf-129">Read-only.</span></span> <span data-ttu-id="28dcf-130">Die Id der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-130">The id of the role assignment request.</span></span>|
|<span data-ttu-id="28dcf-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="28dcf-131">assignmentState</span></span>|<span data-ttu-id="28dcf-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-132">String</span></span>| <span data-ttu-id="28dcf-133">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-133">The state of the assignment.</span></span> <span data-ttu-id="28dcf-134">Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="28dcf-134">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="28dcf-135">duration</span><span class="sxs-lookup"><span data-stu-id="28dcf-135">duration</span></span>|<span data-ttu-id="28dcf-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-136">String</span></span>| <span data-ttu-id="28dcf-137">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-137">The duration of a role assignment.</span></span>|
|<span data-ttu-id="28dcf-138">Grund</span><span class="sxs-lookup"><span data-stu-id="28dcf-138">reason</span></span>|<span data-ttu-id="28dcf-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-139">String</span></span>| <span data-ttu-id="28dcf-140">Der Grund für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-140">The reason for the role assignment.</span></span>|
|<span data-ttu-id="28dcf-141">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="28dcf-141">requestedDateTime</span></span>|<span data-ttu-id="28dcf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28dcf-142">DateTimeOffset</span></span>| <span data-ttu-id="28dcf-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="28dcf-143">Read-only.</span></span> <span data-ttu-id="28dcf-144">Die Zeit zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="28dcf-144">The request create time.</span></span> <span data-ttu-id="28dcf-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="28dcf-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="28dcf-146">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="28dcf-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="28dcf-147">roleId</span><span class="sxs-lookup"><span data-stu-id="28dcf-147">roleId</span></span>|<span data-ttu-id="28dcf-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-148">String</span></span>| <span data-ttu-id="28dcf-149">Die Id der Rolle.</span><span class="sxs-lookup"><span data-stu-id="28dcf-149">The id of the role.</span></span>|
|<span data-ttu-id="28dcf-150">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="28dcf-150">schedule</span></span>|[<span data-ttu-id="28dcf-151">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28dcf-151">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="28dcf-152">Das der Rolle Zuordnung Anforderung Zeitplan-Objekt.</span><span class="sxs-lookup"><span data-stu-id="28dcf-152">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="28dcf-153">status</span><span class="sxs-lookup"><span data-stu-id="28dcf-153">status</span></span>|<span data-ttu-id="28dcf-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-154">String</span></span>| <span data-ttu-id="28dcf-155">Lesen vorbehalten Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="28dcf-155">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="28dcf-156">Der Wert kann sein `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="28dcf-156">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="28dcf-157">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="28dcf-157">ticketNumber</span></span>|<span data-ttu-id="28dcf-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-158">String</span></span>| <span data-ttu-id="28dcf-159">Die TicketNumber für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-159">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="28dcf-160">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="28dcf-160">ticketSystem</span></span>|<span data-ttu-id="28dcf-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-161">String</span></span>| <span data-ttu-id="28dcf-162">Die TicketSystem für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-162">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="28dcf-163">type</span><span class="sxs-lookup"><span data-stu-id="28dcf-163">type</span></span>|<span data-ttu-id="28dcf-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-164">String</span></span>| <span data-ttu-id="28dcf-165">Darstellen der den Typ des Vorgangs für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-165">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="28dcf-166">Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="28dcf-166">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="28dcf-167">userId</span><span class="sxs-lookup"><span data-stu-id="28dcf-167">userId</span></span>|<span data-ttu-id="28dcf-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28dcf-168">String</span></span>| <span data-ttu-id="28dcf-169">Die Id des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="28dcf-169">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28dcf-170">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="28dcf-170">Relationships</span></span>
| <span data-ttu-id="28dcf-171">Beziehung</span><span class="sxs-lookup"><span data-stu-id="28dcf-171">Relationship</span></span> | <span data-ttu-id="28dcf-172">Typ</span><span class="sxs-lookup"><span data-stu-id="28dcf-172">Type</span></span>        | <span data-ttu-id="28dcf-173">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28dcf-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28dcf-174">roleInfo</span><span class="sxs-lookup"><span data-stu-id="28dcf-174">roleInfo</span></span>|[<span data-ttu-id="28dcf-175">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="28dcf-175">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="28dcf-176">Das Objekt RoleInfo der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28dcf-176">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28dcf-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28dcf-177">JSON representation</span></span>

<span data-ttu-id="28dcf-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28dcf-178">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
