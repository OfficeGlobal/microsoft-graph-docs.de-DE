---
title: Erstellen von privilegedRoleAssignmentRequest
description: Erstellen Sie ein Privilegedroleassignmentrequest-Objekt.
localization_priority: Normal
ms.openlocfilehash: 3f1b88415e5671e38ad557cc28200569a42a9630
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847769"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="22d68-103">Erstellen von privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-103">Create privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="22d68-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22d68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22d68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22d68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22d68-106">Erstellen Sie ein [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="22d68-106">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22d68-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="22d68-107">Permissions</span></span>
<span data-ttu-id="22d68-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22d68-110">Permission type</span></span>                        | <span data-ttu-id="22d68-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22d68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="22d68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22d68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22d68-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22d68-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22d68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22d68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22d68-115">Not supported.</span></span> |
|<span data-ttu-id="22d68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22d68-116">Application</span></span>                            | <span data-ttu-id="22d68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22d68-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22d68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22d68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="22d68-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22d68-119">Request headers</span></span>
| <span data-ttu-id="22d68-120">Name</span><span class="sxs-lookup"><span data-stu-id="22d68-120">Name</span></span>      |<span data-ttu-id="22d68-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22d68-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22d68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d68-122">Authorization</span></span>  | <span data-ttu-id="22d68-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22d68-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22d68-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22d68-125">Request body</span></span>
<span data-ttu-id="22d68-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="22d68-126">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="22d68-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22d68-127">Property</span></span>     | <span data-ttu-id="22d68-128">Typ</span><span class="sxs-lookup"><span data-stu-id="22d68-128">Type</span></span>    |  <span data-ttu-id="22d68-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22d68-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d68-130">roleId</span><span class="sxs-lookup"><span data-stu-id="22d68-130">roleId</span></span>|<span data-ttu-id="22d68-131">String</span><span class="sxs-lookup"><span data-stu-id="22d68-131">String</span></span>|<span data-ttu-id="22d68-132">Die ID der Rolle.</span><span class="sxs-lookup"><span data-stu-id="22d68-132">The ID of the role.</span></span> <span data-ttu-id="22d68-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22d68-133">Required.</span></span>|
|<span data-ttu-id="22d68-134">type</span><span class="sxs-lookup"><span data-stu-id="22d68-134">type</span></span>|<span data-ttu-id="22d68-135">String</span><span class="sxs-lookup"><span data-stu-id="22d68-135">String</span></span>|<span data-ttu-id="22d68-136">Stellt die den Typ des Vorgangs für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="22d68-136">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="22d68-137">Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="22d68-137">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="22d68-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22d68-138">Required.</span></span>|
|<span data-ttu-id="22d68-139">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22d68-139">assignmentState</span></span>|<span data-ttu-id="22d68-140">String</span><span class="sxs-lookup"><span data-stu-id="22d68-140">String</span></span>|<span data-ttu-id="22d68-141">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="22d68-141">The state of the assignment.</span></span> <span data-ttu-id="22d68-142">Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="22d68-142">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="22d68-143">Mögliche Werte: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="22d68-143">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="22d68-144">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22d68-144">Required.</span></span>|
|<span data-ttu-id="22d68-145">Grund</span><span class="sxs-lookup"><span data-stu-id="22d68-145">reason</span></span>|<span data-ttu-id="22d68-146">String</span><span class="sxs-lookup"><span data-stu-id="22d68-146">String</span></span>|<span data-ttu-id="22d68-147">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="22d68-147">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="22d68-148">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="22d68-148">schedule</span></span>|[<span data-ttu-id="22d68-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22d68-149">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="22d68-150">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22d68-150">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="22d68-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="22d68-151">Response</span></span>
<span data-ttu-id="22d68-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="22d68-152">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="22d68-153">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="22d68-153">Error codes</span></span>
<span data-ttu-id="22d68-154">Diese API gibt den betreffenden Standard-HTTP-Fehlercodes.</span><span class="sxs-lookup"><span data-stu-id="22d68-154">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="22d68-155">Darüber hinaus kann die Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="22d68-155">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="22d68-156">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="22d68-156">Error code</span></span>     | <span data-ttu-id="22d68-157">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="22d68-157">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="22d68-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-158">400 BadRequest</span></span> | <span data-ttu-id="22d68-159">RoleAssignmentRequest-Eigenschaft wurde NULL</span><span class="sxs-lookup"><span data-stu-id="22d68-159">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="22d68-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-160">400 BadRequest</span></span> | <span data-ttu-id="22d68-161">Kann nicht RoleAssignmentRequest Objekt deserialisiert werden.</span><span class="sxs-lookup"><span data-stu-id="22d68-161">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="22d68-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-162">400 BadRequest</span></span> | <span data-ttu-id="22d68-163">RoleId ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22d68-163">RoleId is required.</span></span> |
| <span data-ttu-id="22d68-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-164">400 BadRequest</span></span> | <span data-ttu-id="22d68-165">Startdatum muss angegeben werden und sollte jetzt größer sein.</span><span class="sxs-lookup"><span data-stu-id="22d68-165">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="22d68-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-166">400 BadRequest</span></span> | <span data-ttu-id="22d68-167">Ein Zeitplan für diesen Benutzer, Rollen und Zeitplan ist bereits vorhanden.</span><span class="sxs-lookup"><span data-stu-id="22d68-167">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="22d68-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-168">400 BadRequest</span></span> | <span data-ttu-id="22d68-169">Für diesen Benutzer, Rollen und Genehmigung ist eine ausstehende Genehmigung bereits vorhanden.</span><span class="sxs-lookup"><span data-stu-id="22d68-169">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="22d68-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-170">400 BadRequest</span></span> | <span data-ttu-id="22d68-171">Requestor Grund ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="22d68-171">Requestor reason is missing.</span></span> |
| <span data-ttu-id="22d68-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-172">400 BadRequest</span></span> | <span data-ttu-id="22d68-173">Requestor Grund sollten weniger als 500 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="22d68-173">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="22d68-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-174">400 BadRequest</span></span> | <span data-ttu-id="22d68-175">Elevation-Dauer muss zwischen 0,5 und {von Einstellung} sein.</span><span class="sxs-lookup"><span data-stu-id="22d68-175">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="22d68-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-176">400 BadRequest</span></span> | <span data-ttu-id="22d68-177">Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22d68-177">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="22d68-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-178">400 BadRequest</span></span> | <span data-ttu-id="22d68-179">Die Rolle ist bereits aktiviert.</span><span class="sxs-lookup"><span data-stu-id="22d68-179">The role is already activated.</span></span> |
| <span data-ttu-id="22d68-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-180">400 BadRequest</span></span> | <span data-ttu-id="22d68-181">GenericElevateUserToRoleAssignments: Tickting Informationen ist erforderlich und nicht in der Aktivierungsprozess angegeben.</span><span class="sxs-lookup"><span data-stu-id="22d68-181">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="22d68-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22d68-182">400 BadRequest</span></span> | <span data-ttu-id="22d68-183">Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22d68-183">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="22d68-184">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="22d68-184">403 UnAuthorized</span></span> | <span data-ttu-id="22d68-185">Elevation erfordert Multi-Factor Authentication.</span><span class="sxs-lookup"><span data-stu-id="22d68-185">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="22d68-186">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="22d68-186">403 UnAuthorized</span></span> | <span data-ttu-id="22d68-187">Im Namen Elevation ist nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="22d68-187">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="22d68-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22d68-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22d68-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22d68-189">Request</span></span>
<span data-ttu-id="22d68-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22d68-190">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a><span data-ttu-id="22d68-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="22d68-191">Response</span></span>
<span data-ttu-id="22d68-192">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="22d68-192">The following is an example of the response.</span></span> <span data-ttu-id="22d68-193">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="22d68-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22d68-194">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22d68-194">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
