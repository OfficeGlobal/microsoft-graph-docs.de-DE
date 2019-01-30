---
title: Erstellen von privilegedRoleAssignmentRequest
description: Erstellen Sie ein Privilegedroleassignmentrequest-Objekt.
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641687"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="ae507-103">Erstellen von privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae507-104">Erstellen Sie ein [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="ae507-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae507-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae507-105">Permissions</span></span>
<span data-ttu-id="ae507-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae507-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae507-108">Permission type</span></span>                        | <span data-ttu-id="ae507-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae507-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae507-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae507-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae507-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae507-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae507-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae507-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae507-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae507-113">Not supported.</span></span> |
|<span data-ttu-id="ae507-114">Application</span><span class="sxs-lookup"><span data-stu-id="ae507-114">Application</span></span>                            | <span data-ttu-id="ae507-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae507-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae507-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae507-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="ae507-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae507-117">Request headers</span></span>
| <span data-ttu-id="ae507-118">Name</span><span class="sxs-lookup"><span data-stu-id="ae507-118">Name</span></span>      |<span data-ttu-id="ae507-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae507-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae507-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae507-120">Authorization</span></span>  | <span data-ttu-id="ae507-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae507-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae507-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae507-123">Request body</span></span>
<span data-ttu-id="ae507-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae507-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="ae507-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae507-125">Property</span></span>     | <span data-ttu-id="ae507-126">Typ</span><span class="sxs-lookup"><span data-stu-id="ae507-126">Type</span></span>    |  <span data-ttu-id="ae507-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae507-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae507-128">roleId</span><span class="sxs-lookup"><span data-stu-id="ae507-128">roleId</span></span>|<span data-ttu-id="ae507-129">String</span><span class="sxs-lookup"><span data-stu-id="ae507-129">String</span></span>|<span data-ttu-id="ae507-130">Die ID der Rolle.</span><span class="sxs-lookup"><span data-stu-id="ae507-130">The ID of the role.</span></span> <span data-ttu-id="ae507-131">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae507-131">Required.</span></span>|
|<span data-ttu-id="ae507-132">type</span><span class="sxs-lookup"><span data-stu-id="ae507-132">type</span></span>|<span data-ttu-id="ae507-133">String</span><span class="sxs-lookup"><span data-stu-id="ae507-133">String</span></span>|<span data-ttu-id="ae507-134">Stellt die den Typ des Vorgangs für die rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="ae507-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="ae507-135">Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen.</span><span class="sxs-lookup"><span data-stu-id="ae507-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="ae507-136">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ae507-136">Required.</span></span>|
|<span data-ttu-id="ae507-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="ae507-137">assignmentState</span></span>|<span data-ttu-id="ae507-138">String</span><span class="sxs-lookup"><span data-stu-id="ae507-138">String</span></span>|<span data-ttu-id="ae507-139">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="ae507-139">The state of the assignment.</span></span> <span data-ttu-id="ae507-140">Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ae507-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="ae507-141">Mögliche Werte: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="ae507-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="ae507-142">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ae507-142">Required.</span></span>|
|<span data-ttu-id="ae507-143">Grund</span><span class="sxs-lookup"><span data-stu-id="ae507-143">reason</span></span>|<span data-ttu-id="ae507-144">String</span><span class="sxs-lookup"><span data-stu-id="ae507-144">String</span></span>|<span data-ttu-id="ae507-145">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="ae507-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="ae507-146">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="ae507-146">schedule</span></span>|[<span data-ttu-id="ae507-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ae507-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="ae507-148">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae507-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="ae507-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae507-149">Response</span></span>
<span data-ttu-id="ae507-150">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae507-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="ae507-151">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="ae507-151">Error codes</span></span>
<span data-ttu-id="ae507-152">Diese API gibt den betreffenden Standard-HTTP-Fehlercodes.</span><span class="sxs-lookup"><span data-stu-id="ae507-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="ae507-153">Darüber hinaus kann die Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ae507-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="ae507-154">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="ae507-154">Error code</span></span>     | <span data-ttu-id="ae507-155">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="ae507-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="ae507-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-156">400 BadRequest</span></span> | <span data-ttu-id="ae507-157">RoleAssignmentRequest-Eigenschaft wurde NULL</span><span class="sxs-lookup"><span data-stu-id="ae507-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="ae507-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-158">400 BadRequest</span></span> | <span data-ttu-id="ae507-159">Kann nicht RoleAssignmentRequest Objekt deserialisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ae507-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="ae507-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-160">400 BadRequest</span></span> | <span data-ttu-id="ae507-161">RoleId ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae507-161">RoleId is required.</span></span> |
| <span data-ttu-id="ae507-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-162">400 BadRequest</span></span> | <span data-ttu-id="ae507-163">Startdatum muss angegeben werden und sollte jetzt größer sein.</span><span class="sxs-lookup"><span data-stu-id="ae507-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="ae507-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-164">400 BadRequest</span></span> | <span data-ttu-id="ae507-165">Ein Zeitplan für diesen Benutzer, Rollen und Zeitplan ist bereits vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ae507-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="ae507-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-166">400 BadRequest</span></span> | <span data-ttu-id="ae507-167">Für diesen Benutzer, Rollen und Genehmigung ist eine ausstehende Genehmigung bereits vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ae507-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="ae507-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-168">400 BadRequest</span></span> | <span data-ttu-id="ae507-169">Requestor Grund ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ae507-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="ae507-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-170">400 BadRequest</span></span> | <span data-ttu-id="ae507-171">Requestor Grund sollten weniger als 500 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="ae507-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="ae507-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-172">400 BadRequest</span></span> | <span data-ttu-id="ae507-173">Elevation-Dauer muss zwischen 0,5 und {von Einstellung} sein.</span><span class="sxs-lookup"><span data-stu-id="ae507-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="ae507-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-174">400 BadRequest</span></span> | <span data-ttu-id="ae507-175">Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae507-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="ae507-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-176">400 BadRequest</span></span> | <span data-ttu-id="ae507-177">Die Rolle ist bereits aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ae507-177">The role is already activated.</span></span> |
| <span data-ttu-id="ae507-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-178">400 BadRequest</span></span> | <span data-ttu-id="ae507-179">GenericElevateUserToRoleAssignments: Tickting Informationen ist erforderlich und nicht in der Aktivierungsprozess angegeben.</span><span class="sxs-lookup"><span data-stu-id="ae507-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="ae507-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ae507-180">400 BadRequest</span></span> | <span data-ttu-id="ae507-181">Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae507-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="ae507-182">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="ae507-182">403 UnAuthorized</span></span> | <span data-ttu-id="ae507-183">Elevation erfordert Multi-Factor Authentication.</span><span class="sxs-lookup"><span data-stu-id="ae507-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="ae507-184">403 nicht autorisiert</span><span class="sxs-lookup"><span data-stu-id="ae507-184">403 UnAuthorized</span></span> | <span data-ttu-id="ae507-185">Im Namen Elevation ist nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="ae507-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="ae507-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae507-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae507-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae507-187">Request</span></span>
<span data-ttu-id="ae507-188">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae507-188">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ae507-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae507-189">Response</span></span>
<span data-ttu-id="ae507-190">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae507-190">The following is an example of the response.</span></span> <span data-ttu-id="ae507-191">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ae507-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ae507-192">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae507-192">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
