---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061016"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="4d5b6-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="4d5b6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d5b6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d5b6-107">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="4d5b6-108">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-108">The following table lists the operations.</span></span>

| <span data-ttu-id="4d5b6-109">Vorgang</span><span class="sxs-lookup"><span data-stu-id="4d5b6-109">Operation</span></span>       | <span data-ttu-id="4d5b6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="4d5b6-111">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-111">Assign a role assignment</span></span>| <span data-ttu-id="4d5b6-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="4d5b6-112">AdminAdd</span></span> |
| <span data-ttu-id="4d5b6-113">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="4d5b6-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="4d5b6-114">UserAdd</span></span> | 
| <span data-ttu-id="4d5b6-115">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="4d5b6-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="4d5b6-116">UserRemove</span></span> | 
| <span data-ttu-id="4d5b6-117">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-117">Remove a role assignment</span></span>| <span data-ttu-id="4d5b6-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="4d5b6-118">AdminRemove</span></span> |
| <span data-ttu-id="4d5b6-119">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-119">Update a role assignment</span></span>| <span data-ttu-id="4d5b6-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="4d5b6-120">AdminUpdate</span></span> |
| <span data-ttu-id="4d5b6-121">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="4d5b6-121">Request to extend my role assignment</span></span>| <span data-ttu-id="4d5b6-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="4d5b6-122">UserExtend</span></span> | 
| <span data-ttu-id="4d5b6-123">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-123">Extend a role assignment</span></span>| <span data-ttu-id="4d5b6-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="4d5b6-124">AdminExtend</span></span> | 
| <span data-ttu-id="4d5b6-125">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="4d5b6-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="4d5b6-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="4d5b6-126">UserRenew</span></span> | 
| <span data-ttu-id="4d5b6-127">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-127">Renew an expired role assignment</span></span>| <span data-ttu-id="4d5b6-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="4d5b6-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="4d5b6-129">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d5b6-129">Permissions</span></span>
<span data-ttu-id="4d5b6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d5b6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d5b6-132">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d5b6-132">Permission type</span></span>      | <span data-ttu-id="4d5b6-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d5b6-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d5b6-134">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d5b6-134">Delegated (work or school account)</span></span> | <span data-ttu-id="4d5b6-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4d5b6-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="4d5b6-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d5b6-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d5b6-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d5b6-137">Not supported.</span></span>    |
|<span data-ttu-id="4d5b6-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-138">Application</span></span> | <span data-ttu-id="4d5b6-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4d5b6-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d5b6-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d5b6-141">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4d5b6-141">Optional query parameters</span></span>
<span data-ttu-id="4d5b6-142">Diese Methode keine [OData-Abfrage-Parameter](/graph/query-parameters) **nicht** unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-142">This method does **not** support [OData query parameters](/graph/query-parameters).</span></span>

### <a name="request-headers"></a><span data-ttu-id="4d5b6-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d5b6-143">Request headers</span></span>
| <span data-ttu-id="4d5b6-144">Name</span><span class="sxs-lookup"><span data-stu-id="4d5b6-144">Name</span></span>       | <span data-ttu-id="4d5b6-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d5b6-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d5b6-146">Authorization</span></span>  | <span data-ttu-id="4d5b6-147">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4d5b6-147">Bearer {code}</span></span>|
| <span data-ttu-id="4d5b6-148">Content-type</span><span class="sxs-lookup"><span data-stu-id="4d5b6-148">Content-type</span></span>  | <span data-ttu-id="4d5b6-149">application/json</span><span class="sxs-lookup"><span data-stu-id="4d5b6-149">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="4d5b6-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d5b6-150">Request body</span></span>
<span data-ttu-id="4d5b6-151">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-151">In the request body, supply a JSON representation of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="4d5b6-152">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-152">Property</span></span>     | <span data-ttu-id="4d5b6-153">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-153">Type</span></span>    |<span data-ttu-id="4d5b6-154">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-154">Required</span></span>|  <span data-ttu-id="4d5b6-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-155">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-156">resourceId</span></span>|<span data-ttu-id="4d5b6-157">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-157">String</span></span>|<span data-ttu-id="4d5b6-158">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-158">Yes</span></span>|<span data-ttu-id="4d5b6-159">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-159">The ID of the resource.</span></span>|
|<span data-ttu-id="4d5b6-160">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-160">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-161">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-161">String</span></span>|<span data-ttu-id="4d5b6-162">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-162">Yes</span></span>|<span data-ttu-id="4d5b6-163">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-163">The ID of the role definition.</span></span>|
|<span data-ttu-id="4d5b6-164">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-164">subjectId</span></span>|<span data-ttu-id="4d5b6-165">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-165">String</span></span>|<span data-ttu-id="4d5b6-166">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-166">Yes</span></span>|<span data-ttu-id="4d5b6-167">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-167">The ID of the subject.</span></span>|
|<span data-ttu-id="4d5b6-168">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-168">assignmentState</span></span>|<span data-ttu-id="4d5b6-169">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-169">String</span></span>|<span data-ttu-id="4d5b6-170">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-170">Yes</span></span>|<span data-ttu-id="4d5b6-171">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-171">The state of assignment.</span></span> <span data-ttu-id="4d5b6-172">Der Wert kann sein ``Eligible`` und ``Active``.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-172">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="4d5b6-173">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-173">type</span></span>|<span data-ttu-id="4d5b6-174">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-174">String</span></span>|<span data-ttu-id="4d5b6-175">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-175">Yes</span></span>|<span data-ttu-id="4d5b6-176">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-176">The request type.</span></span> <span data-ttu-id="4d5b6-177">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-177">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="4d5b6-178">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-178">reason</span></span>|<span data-ttu-id="4d5b6-179">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-179">String</span></span>| |<span data-ttu-id="4d5b6-180">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-180">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="4d5b6-181">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-181">schedule</span></span>|[<span data-ttu-id="4d5b6-182">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-182">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="4d5b6-183">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-183">The schedule of the role assignment request.</span></span> <span data-ttu-id="4d5b6-184">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-184">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

### <a name="response"></a><span data-ttu-id="4d5b6-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-185">Response</span></span>
<span data-ttu-id="4d5b6-186">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-186">If successful, this method returns a `201, Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="error-codes"></a><span data-ttu-id="4d5b6-187">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="4d5b6-187">Error codes</span></span>
<span data-ttu-id="4d5b6-188">Diese API folgt dem Standard von HTTP-Codes, zusätzlich zu den Fehlercodes, die in der folgenden Tabelle aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-188">This API follows the standard of HTTP codes, in addition to the error codes listed in the following table.</span></span>

|<span data-ttu-id="4d5b6-189">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="4d5b6-189">Error code</span></span>     | <span data-ttu-id="4d5b6-190">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-190">Error message</span></span>              | <span data-ttu-id="4d5b6-191">Details</span><span class="sxs-lookup"><span data-stu-id="4d5b6-191">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="4d5b6-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-192">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-193">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="4d5b6-193">RoleNotFound</span></span>    | <span data-ttu-id="4d5b6-194">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-194">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="4d5b6-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-195">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-196">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="4d5b6-196">ResourceIsLocked</span></span>    | <span data-ttu-id="4d5b6-197">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-197">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="4d5b6-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-198">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-199">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="4d5b6-199">SubjectNotFound</span></span>    | <span data-ttu-id="4d5b6-200">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-200">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="4d5b6-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-201">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-202">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-202">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="4d5b6-203">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-203">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="4d5b6-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-204">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-205">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="4d5b6-205">RoleAssignmentExists</span></span>    | <span data-ttu-id="4d5b6-206">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="4d5b6-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-207">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-208">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="4d5b6-208">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="4d5b6-209">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-209">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="4d5b6-210">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4d5b6-210">400 BadRequest</span></span> | <span data-ttu-id="4d5b6-211">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="4d5b6-211">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="4d5b6-212">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-212">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="example-1"></a><span data-ttu-id="4d5b6-213">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="4d5b6-213">Example 1</span></span>
<span data-ttu-id="4d5b6-214">In diesem Beispiel weisen Sie Administratoren Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-214">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="4d5b6-215">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-215">**Note:** Besides the permission, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="4d5b6-216">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-216">Property</span></span>     | <span data-ttu-id="4d5b6-217">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-217">Type</span></span>    |<span data-ttu-id="4d5b6-218">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-218">Required</span></span>|  <span data-ttu-id="4d5b6-219">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-219">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-220">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-220">resourceId</span></span>|<span data-ttu-id="4d5b6-221">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-221">String</span></span>|<span data-ttu-id="4d5b6-222">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-222">Yes</span></span>|<span data-ttu-id="4d5b6-223">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-223">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-224">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-224">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-225">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-225">String</span></span>|<span data-ttu-id="4d5b6-226">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-226">Yes</span></span>|<span data-ttu-id="4d5b6-227">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-227">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-228">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-228">subjectId</span></span>|<span data-ttu-id="4d5b6-229">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-229">String</span></span>|<span data-ttu-id="4d5b6-230">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-230">Yes</span></span>|<span data-ttu-id="4d5b6-231">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-231">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-232">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-232">assignmentState</span></span>|<span data-ttu-id="4d5b6-233">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-233">String</span></span>|<span data-ttu-id="4d5b6-234">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-234">Yes</span></span>| <span data-ttu-id="4d5b6-235">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="4d5b6-235">Eligible / Active</span></span>|
|<span data-ttu-id="4d5b6-236">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-236">type</span></span>|<span data-ttu-id="4d5b6-237">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-237">String</span></span>|<span data-ttu-id="4d5b6-238">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-238">Yes</span></span>| <span data-ttu-id="4d5b6-239">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="4d5b6-239">AdminAdd</span></span>|
|<span data-ttu-id="4d5b6-240">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-240">reason</span></span>|<span data-ttu-id="4d5b6-241">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-241">String</span></span>| <span data-ttu-id="4d5b6-242">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="4d5b6-242">depends on role Settings</span></span>||
|<span data-ttu-id="4d5b6-243">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-243">schedule</span></span>|[<span data-ttu-id="4d5b6-244">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-244">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-245">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-245">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-246">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-246">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-247">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

## <a name="example-2"></a><span data-ttu-id="4d5b6-248">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="4d5b6-248">Example 2</span></span>
<span data-ttu-id="4d5b6-249">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="4d5b6-250">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-250">Property</span></span>     | <span data-ttu-id="4d5b6-251">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-251">Type</span></span>    |<span data-ttu-id="4d5b6-252">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-252">Required</span></span>|  <span data-ttu-id="4d5b6-253">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-253">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-254">resourceId</span></span>|<span data-ttu-id="4d5b6-255">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-255">String</span></span>|<span data-ttu-id="4d5b6-256">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-256">Yes</span></span>|<span data-ttu-id="4d5b6-257">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-257">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-258">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-258">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-259">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-259">String</span></span>|<span data-ttu-id="4d5b6-260">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-260">Yes</span></span>|<span data-ttu-id="4d5b6-261">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-261">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-262">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-262">subjectId</span></span>|<span data-ttu-id="4d5b6-263">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-263">String</span></span>|<span data-ttu-id="4d5b6-264">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-264">Yes</span></span>|<span data-ttu-id="4d5b6-265">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-265">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-266">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-266">assignmentState</span></span>|<span data-ttu-id="4d5b6-267">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-267">String</span></span>|<span data-ttu-id="4d5b6-268">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-268">Yes</span></span>| <span data-ttu-id="4d5b6-269">Aktiv</span><span class="sxs-lookup"><span data-stu-id="4d5b6-269">Active</span></span>|
|<span data-ttu-id="4d5b6-270">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-270">type</span></span>|<span data-ttu-id="4d5b6-271">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-271">String</span></span>|<span data-ttu-id="4d5b6-272">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-272">Yes</span></span>| <span data-ttu-id="4d5b6-273">UserAdd</span><span class="sxs-lookup"><span data-stu-id="4d5b6-273">UserAdd</span></span>|
|<span data-ttu-id="4d5b6-274">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-274">reason</span></span>|<span data-ttu-id="4d5b6-275">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-275">String</span></span>| <span data-ttu-id="4d5b6-276">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="4d5b6-276">depends on role Settings</span></span>||
|<span data-ttu-id="4d5b6-277">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-277">schedule</span></span>|[<span data-ttu-id="4d5b6-278">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-278">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-279">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-279">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-280">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-280">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-281">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-281">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

## <a name="example-3"></a><span data-ttu-id="4d5b6-282">Beispiel 3</span><span class="sxs-lookup"><span data-stu-id="4d5b6-282">Example 3</span></span>
<span data-ttu-id="4d5b6-283">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-283">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="4d5b6-284">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-284">Property</span></span>     | <span data-ttu-id="4d5b6-285">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-285">Type</span></span>    |<span data-ttu-id="4d5b6-286">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-286">Required</span></span>|  <span data-ttu-id="4d5b6-287">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-287">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-288">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-288">resourceId</span></span>|<span data-ttu-id="4d5b6-289">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-289">String</span></span>|<span data-ttu-id="4d5b6-290">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-290">Yes</span></span>|<span data-ttu-id="4d5b6-291">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-291">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-292">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-292">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-293">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-293">String</span></span>|<span data-ttu-id="4d5b6-294">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-294">Yes</span></span>|<span data-ttu-id="4d5b6-295">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-295">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-296">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-296">subjectId</span></span>|<span data-ttu-id="4d5b6-297">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-297">String</span></span>|<span data-ttu-id="4d5b6-298">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-298">Yes</span></span>|<span data-ttu-id="4d5b6-299">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-299">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-300">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-300">assignmentState</span></span>|<span data-ttu-id="4d5b6-301">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-301">String</span></span>|<span data-ttu-id="4d5b6-302">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-302">Yes</span></span>| <span data-ttu-id="4d5b6-303">Aktiv</span><span class="sxs-lookup"><span data-stu-id="4d5b6-303">Active</span></span>|
|<span data-ttu-id="4d5b6-304">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-304">type</span></span>|<span data-ttu-id="4d5b6-305">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-305">String</span></span>|<span data-ttu-id="4d5b6-306">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-306">Yes</span></span>| <span data-ttu-id="4d5b6-307">UserRemove</span><span class="sxs-lookup"><span data-stu-id="4d5b6-307">UserRemove</span></span>|
|<span data-ttu-id="4d5b6-308">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-308">reason</span></span>|<span data-ttu-id="4d5b6-309">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-309">String</span></span>| <span data-ttu-id="4d5b6-310">Nein</span><span class="sxs-lookup"><span data-stu-id="4d5b6-310">No</span></span>||
|<span data-ttu-id="4d5b6-311">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-311">schedule</span></span>|[<span data-ttu-id="4d5b6-312">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-312">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-313">Nein</span><span class="sxs-lookup"><span data-stu-id="4d5b6-313">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-314">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-314">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-315">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-315">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="4d5b6-316">Beispiel 4</span><span class="sxs-lookup"><span data-stu-id="4d5b6-316">Example 4</span></span>
<span data-ttu-id="4d5b6-317">In diesem Beispiel Entfernen von Administratoren die nawu@fimdev.net Benutzer aus der Rolle Leser Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-317">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="4d5b6-318">**Hinweis:** Neben den Berechtigungsbereich erfordert in diesem Beispiel wird den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-318">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="4d5b6-319">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-319">Property</span></span>     | <span data-ttu-id="4d5b6-320">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-320">Type</span></span>    |<span data-ttu-id="4d5b6-321">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-321">Required</span></span>|  <span data-ttu-id="4d5b6-322">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-322">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-323">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-323">resourceId</span></span>|<span data-ttu-id="4d5b6-324">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-324">String</span></span>|<span data-ttu-id="4d5b6-325">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-325">Yes</span></span>|<span data-ttu-id="4d5b6-326">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-326">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-327">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-327">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-328">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-328">String</span></span>|<span data-ttu-id="4d5b6-329">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-329">Yes</span></span>|<span data-ttu-id="4d5b6-330">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-330">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-331">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-331">subjectId</span></span>|<span data-ttu-id="4d5b6-332">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-332">String</span></span>|<span data-ttu-id="4d5b6-333">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-333">Yes</span></span>|<span data-ttu-id="4d5b6-334">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-334">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-335">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-335">assignmentState</span></span>|<span data-ttu-id="4d5b6-336">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-336">String</span></span>|<span data-ttu-id="4d5b6-337">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-337">Yes</span></span>| <span data-ttu-id="4d5b6-338">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="4d5b6-338">Eligible / Active</span></span>|
|<span data-ttu-id="4d5b6-339">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-339">type</span></span>|<span data-ttu-id="4d5b6-340">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-340">String</span></span>|<span data-ttu-id="4d5b6-341">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-341">Yes</span></span>| <span data-ttu-id="4d5b6-342">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="4d5b6-342">AdminRemove</span></span>|
|<span data-ttu-id="4d5b6-343">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-343">reason</span></span>|<span data-ttu-id="4d5b6-344">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-344">String</span></span>| <span data-ttu-id="4d5b6-345">Nein</span><span class="sxs-lookup"><span data-stu-id="4d5b6-345">No</span></span>||
|<span data-ttu-id="4d5b6-346">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-346">schedule</span></span>|[<span data-ttu-id="4d5b6-347">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-347">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-348">Nein</span><span class="sxs-lookup"><span data-stu-id="4d5b6-348">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-349">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-349">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-350">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-350">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="4d5b6-351">Beispiel 5</span><span class="sxs-lookup"><span data-stu-id="4d5b6-351">Example 5</span></span>
<span data-ttu-id="4d5b6-352">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-352">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="4d5b6-353">**Hinweis:** Neben den Berechtigungsbereich erfordert in diesem Beispiel wird den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-353">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 
| <span data-ttu-id="4d5b6-354">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-354">Property</span></span>     | <span data-ttu-id="4d5b6-355">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-355">Type</span></span>    |<span data-ttu-id="4d5b6-356">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-356">Required</span></span>|  <span data-ttu-id="4d5b6-357">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-357">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-358">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-358">resourceId</span></span>|<span data-ttu-id="4d5b6-359">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-359">String</span></span>|<span data-ttu-id="4d5b6-360">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-360">Yes</span></span>|<span data-ttu-id="4d5b6-361">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-361">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-362">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-362">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-363">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-363">String</span></span>|<span data-ttu-id="4d5b6-364">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-364">Yes</span></span>|<span data-ttu-id="4d5b6-365">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-365">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-366">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-366">subjectId</span></span>|<span data-ttu-id="4d5b6-367">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-367">String</span></span>|<span data-ttu-id="4d5b6-368">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-368">Yes</span></span>|<span data-ttu-id="4d5b6-369">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-369">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-370">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-370">assignmentState</span></span>|<span data-ttu-id="4d5b6-371">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-371">String</span></span>|<span data-ttu-id="4d5b6-372">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-372">Yes</span></span>| <span data-ttu-id="4d5b6-373">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="4d5b6-373">Eligible / Active</span></span>|
|<span data-ttu-id="4d5b6-374">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-374">type</span></span>|<span data-ttu-id="4d5b6-375">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-375">String</span></span>|<span data-ttu-id="4d5b6-376">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-376">Yes</span></span>| <span data-ttu-id="4d5b6-377">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="4d5b6-377">AdminUpdate</span></span>|
|<span data-ttu-id="4d5b6-378">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-378">reason</span></span>|<span data-ttu-id="4d5b6-379">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-379">String</span></span>| <span data-ttu-id="4d5b6-380">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="4d5b6-380">depends on roleSettings</span></span>||
|<span data-ttu-id="4d5b6-381">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-381">schedule</span></span>|[<span data-ttu-id="4d5b6-382">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-382">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-383">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-383">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-384">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-384">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-385">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-385">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="4d5b6-386">Beispiel 6</span><span class="sxs-lookup"><span data-stu-id="4d5b6-386">Example 6</span></span>
<span data-ttu-id="4d5b6-387">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-387">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="4d5b6-388">**Hinweis:** Neben den Berechtigungsbereich erfordert in diesem Beispiel wird den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d5b6-388">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="4d5b6-389">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5b6-389">Property</span></span>     | <span data-ttu-id="4d5b6-390">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-390">Type</span></span>    |<span data-ttu-id="4d5b6-391">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5b6-391">Required</span></span>|  <span data-ttu-id="4d5b6-392">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5b6-392">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4d5b6-393">resourceId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-393">resourceId</span></span>|<span data-ttu-id="4d5b6-394">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-394">String</span></span>|<span data-ttu-id="4d5b6-395">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-395">Yes</span></span>|<span data-ttu-id="4d5b6-396">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-396">\<resourceId\></span></span>|
|<span data-ttu-id="4d5b6-397">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-397">roleDefinitionId</span></span>|<span data-ttu-id="4d5b6-398">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-398">String</span></span>|<span data-ttu-id="4d5b6-399">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-399">Yes</span></span>|<span data-ttu-id="4d5b6-400">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-400">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4d5b6-401">subjectId</span><span class="sxs-lookup"><span data-stu-id="4d5b6-401">subjectId</span></span>|<span data-ttu-id="4d5b6-402">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-402">String</span></span>|<span data-ttu-id="4d5b6-403">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-403">Yes</span></span>|<span data-ttu-id="4d5b6-404">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4d5b6-404">\<subjectId\></span></span>|
|<span data-ttu-id="4d5b6-405">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4d5b6-405">assignmentState</span></span>|<span data-ttu-id="4d5b6-406">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-406">String</span></span>|<span data-ttu-id="4d5b6-407">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-407">Yes</span></span>| <span data-ttu-id="4d5b6-408">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="4d5b6-408">Eligible / Active</span></span> |
|<span data-ttu-id="4d5b6-409">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5b6-409">type</span></span>|<span data-ttu-id="4d5b6-410">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-410">String</span></span>|<span data-ttu-id="4d5b6-411">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-411">Yes</span></span>| <span data-ttu-id="4d5b6-412">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="4d5b6-412">AdminExtend</span></span>|
|<span data-ttu-id="4d5b6-413">Grund</span><span class="sxs-lookup"><span data-stu-id="4d5b6-413">reason</span></span>|<span data-ttu-id="4d5b6-414">String</span><span class="sxs-lookup"><span data-stu-id="4d5b6-414">String</span></span>| <span data-ttu-id="4d5b6-415">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="4d5b6-415">depends on roleSettings</span></span>||
|<span data-ttu-id="4d5b6-416">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="4d5b6-416">schedule</span></span>|[<span data-ttu-id="4d5b6-417">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4d5b6-417">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4d5b6-418">Ja</span><span class="sxs-lookup"><span data-stu-id="4d5b6-418">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4d5b6-419">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5b6-419">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="4d5b6-420">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5b6-420">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
