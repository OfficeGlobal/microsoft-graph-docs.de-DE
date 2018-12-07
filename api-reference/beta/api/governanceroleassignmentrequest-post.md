---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
ms.openlocfilehash: 775cc8e22e7d273bfe387e5be2cc183d3d919a38
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191172"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="470c9-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="470c9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="470c9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="470c9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="470c9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="470c9-107">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="470c9-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="470c9-108">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="470c9-108">The following table lists the operations.</span></span>

| <span data-ttu-id="470c9-109">Vorgang</span><span class="sxs-lookup"><span data-stu-id="470c9-109">Operation</span></span>       | <span data-ttu-id="470c9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="470c9-111">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-111">Assign a role assignment</span></span>| <span data-ttu-id="470c9-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="470c9-112">AdminAdd</span></span> |
| <span data-ttu-id="470c9-113">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="470c9-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="470c9-114">UserAdd</span></span> | 
| <span data-ttu-id="470c9-115">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="470c9-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="470c9-116">UserRemove</span></span> | 
| <span data-ttu-id="470c9-117">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-117">Remove a role assignment</span></span>| <span data-ttu-id="470c9-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="470c9-118">AdminRemove</span></span> |
| <span data-ttu-id="470c9-119">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-119">Update a role assignment</span></span>| <span data-ttu-id="470c9-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="470c9-120">AdminUpdate</span></span> |
| <span data-ttu-id="470c9-121">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="470c9-121">Request to extend my role assignment</span></span>| <span data-ttu-id="470c9-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="470c9-122">UserExtend</span></span> | 
| <span data-ttu-id="470c9-123">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-123">Extend a role assignment</span></span>| <span data-ttu-id="470c9-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="470c9-124">AdminExtend</span></span> | 
| <span data-ttu-id="470c9-125">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="470c9-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="470c9-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="470c9-126">UserRenew</span></span> | 
| <span data-ttu-id="470c9-127">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="470c9-127">Renew an expired role assignment</span></span>| <span data-ttu-id="470c9-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="470c9-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="470c9-129">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="470c9-129">Permissions</span></span>
<span data-ttu-id="470c9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="470c9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="470c9-132">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="470c9-132">Permission type</span></span>      | <span data-ttu-id="470c9-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="470c9-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="470c9-134">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="470c9-134">Delegated (work or school account)</span></span> | <span data-ttu-id="470c9-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="470c9-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="470c9-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="470c9-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="470c9-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="470c9-137">Not supported.</span></span>    |
|<span data-ttu-id="470c9-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="470c9-138">Application</span></span> | <span data-ttu-id="470c9-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="470c9-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="470c9-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="470c9-141">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="470c9-141">Request headers</span></span>
| <span data-ttu-id="470c9-142">Name</span><span class="sxs-lookup"><span data-stu-id="470c9-142">Name</span></span>       | <span data-ttu-id="470c9-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="470c9-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="470c9-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="470c9-144">Authorization</span></span>  | <span data-ttu-id="470c9-145">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="470c9-145">Bearer {code}</span></span>|
| <span data-ttu-id="470c9-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="470c9-146">Content-type</span></span>  | <span data-ttu-id="470c9-147">application/json</span><span class="sxs-lookup"><span data-stu-id="470c9-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="470c9-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="470c9-148">Request body</span></span>
<span data-ttu-id="470c9-149">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="470c9-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="470c9-150">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-150">Property</span></span>     | <span data-ttu-id="470c9-151">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-151">Type</span></span>    |<span data-ttu-id="470c9-152">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-152">Required</span></span>|  <span data-ttu-id="470c9-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="470c9-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-154">resourceId</span></span>|<span data-ttu-id="470c9-155">String</span><span class="sxs-lookup"><span data-stu-id="470c9-155">String</span></span>|<span data-ttu-id="470c9-156">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-156">Yes</span></span>|<span data-ttu-id="470c9-157">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="470c9-157">The ID of the resource.</span></span>|
|<span data-ttu-id="470c9-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-158">roleDefinitionId</span></span>|<span data-ttu-id="470c9-159">String</span><span class="sxs-lookup"><span data-stu-id="470c9-159">String</span></span>|<span data-ttu-id="470c9-160">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-160">Yes</span></span>|<span data-ttu-id="470c9-161">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="470c9-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="470c9-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-162">subjectId</span></span>|<span data-ttu-id="470c9-163">String</span><span class="sxs-lookup"><span data-stu-id="470c9-163">String</span></span>|<span data-ttu-id="470c9-164">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-164">Yes</span></span>|<span data-ttu-id="470c9-165">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="470c9-165">The ID of the subject.</span></span>|
|<span data-ttu-id="470c9-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-166">assignmentState</span></span>|<span data-ttu-id="470c9-167">String</span><span class="sxs-lookup"><span data-stu-id="470c9-167">String</span></span>|<span data-ttu-id="470c9-168">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-168">Yes</span></span>|<span data-ttu-id="470c9-169">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="470c9-169">The state of assignment.</span></span> <span data-ttu-id="470c9-170">Der Wert kann sein ``Eligible`` und ``Active``.</span><span class="sxs-lookup"><span data-stu-id="470c9-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="470c9-171">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-171">type</span></span>|<span data-ttu-id="470c9-172">String</span><span class="sxs-lookup"><span data-stu-id="470c9-172">String</span></span>|<span data-ttu-id="470c9-173">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-173">Yes</span></span>|<span data-ttu-id="470c9-174">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="470c9-174">The request type.</span></span> <span data-ttu-id="470c9-175">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="470c9-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="470c9-176">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-176">reason</span></span>|<span data-ttu-id="470c9-177">String</span><span class="sxs-lookup"><span data-stu-id="470c9-177">String</span></span>| |<span data-ttu-id="470c9-178">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="470c9-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="470c9-179">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-179">schedule</span></span>|[<span data-ttu-id="470c9-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="470c9-181">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="470c9-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="470c9-182">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="470c9-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="470c9-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-183">Response</span></span>
<span data-ttu-id="470c9-184">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="470c9-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="470c9-185">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="470c9-185">Error codes</span></span>
<span data-ttu-id="470c9-186">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="470c9-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="470c9-187">Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.</span><span class="sxs-lookup"><span data-stu-id="470c9-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="470c9-188">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="470c9-188">Error code</span></span>     | <span data-ttu-id="470c9-189">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="470c9-189">Error message</span></span>              | <span data-ttu-id="470c9-190">Details</span><span class="sxs-lookup"><span data-stu-id="470c9-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="470c9-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-191">400 BadRequest</span></span> | <span data-ttu-id="470c9-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="470c9-192">RoleNotFound</span></span>    | <span data-ttu-id="470c9-193">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="470c9-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="470c9-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-194">400 BadRequest</span></span> | <span data-ttu-id="470c9-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="470c9-195">ResourceIsLocked</span></span>    | <span data-ttu-id="470c9-196">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="470c9-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="470c9-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-197">400 BadRequest</span></span> | <span data-ttu-id="470c9-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="470c9-198">SubjectNotFound</span></span>    | <span data-ttu-id="470c9-199">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="470c9-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="470c9-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-200">400 BadRequest</span></span> | <span data-ttu-id="470c9-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="470c9-202">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="470c9-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="470c9-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-203">400 BadRequest</span></span> | <span data-ttu-id="470c9-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="470c9-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="470c9-205">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="470c9-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="470c9-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-206">400 BadRequest</span></span> | <span data-ttu-id="470c9-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="470c9-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="470c9-208">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="470c9-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="470c9-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="470c9-209">400 BadRequest</span></span> | <span data-ttu-id="470c9-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="470c9-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="470c9-211">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="470c9-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="470c9-212">Beispiele</span><span class="sxs-lookup"><span data-stu-id="470c9-212">Examples</span></span>
<span data-ttu-id="470c9-213">Die folgenden Beispiele zeigen, wie diese API verwendet.</span><span class="sxs-lookup"><span data-stu-id="470c9-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="470c9-214">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="470c9-214">Example 1</span></span>
<span data-ttu-id="470c9-215">In diesem Beispiel weisen Sie Administratoren Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="470c9-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="470c9-216">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="470c9-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="470c9-217">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-217">Property</span></span>     | <span data-ttu-id="470c9-218">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-218">Type</span></span>    |<span data-ttu-id="470c9-219">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-219">Required</span></span>|  <span data-ttu-id="470c9-220">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-221">resourceId</span></span>|<span data-ttu-id="470c9-222">String</span><span class="sxs-lookup"><span data-stu-id="470c9-222">String</span></span>|<span data-ttu-id="470c9-223">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-223">Yes</span></span>|<span data-ttu-id="470c9-224">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-224">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-225">roleDefinitionId</span></span>|<span data-ttu-id="470c9-226">String</span><span class="sxs-lookup"><span data-stu-id="470c9-226">String</span></span>|<span data-ttu-id="470c9-227">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-227">Yes</span></span>|<span data-ttu-id="470c9-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-229">subjectId</span></span>|<span data-ttu-id="470c9-230">String</span><span class="sxs-lookup"><span data-stu-id="470c9-230">String</span></span>|<span data-ttu-id="470c9-231">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-231">Yes</span></span>|<span data-ttu-id="470c9-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-232">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-233">assignmentState</span></span>|<span data-ttu-id="470c9-234">String</span><span class="sxs-lookup"><span data-stu-id="470c9-234">String</span></span>|<span data-ttu-id="470c9-235">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-235">Yes</span></span>| <span data-ttu-id="470c9-236">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="470c9-236">Eligible / Active</span></span>|
|<span data-ttu-id="470c9-237">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-237">type</span></span>|<span data-ttu-id="470c9-238">String</span><span class="sxs-lookup"><span data-stu-id="470c9-238">String</span></span>|<span data-ttu-id="470c9-239">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-239">Yes</span></span>| <span data-ttu-id="470c9-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="470c9-240">AdminAdd</span></span>|
|<span data-ttu-id="470c9-241">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-241">reason</span></span>|<span data-ttu-id="470c9-242">String</span><span class="sxs-lookup"><span data-stu-id="470c9-242">String</span></span>| <span data-ttu-id="470c9-243">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="470c9-243">depends on role Settings</span></span>||
|<span data-ttu-id="470c9-244">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-244">schedule</span></span>|[<span data-ttu-id="470c9-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-246">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="470c9-249">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="470c9-249">Example 2</span></span>
<span data-ttu-id="470c9-250">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="470c9-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="470c9-251">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-251">Property</span></span>     | <span data-ttu-id="470c9-252">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-252">Type</span></span>    |<span data-ttu-id="470c9-253">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-253">Required</span></span>|  <span data-ttu-id="470c9-254">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-255">resourceId</span></span>|<span data-ttu-id="470c9-256">String</span><span class="sxs-lookup"><span data-stu-id="470c9-256">String</span></span>|<span data-ttu-id="470c9-257">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-257">Yes</span></span>|<span data-ttu-id="470c9-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-258">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-259">roleDefinitionId</span></span>|<span data-ttu-id="470c9-260">String</span><span class="sxs-lookup"><span data-stu-id="470c9-260">String</span></span>|<span data-ttu-id="470c9-261">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-261">Yes</span></span>|<span data-ttu-id="470c9-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-263">subjectId</span></span>|<span data-ttu-id="470c9-264">String</span><span class="sxs-lookup"><span data-stu-id="470c9-264">String</span></span>|<span data-ttu-id="470c9-265">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-265">Yes</span></span>|<span data-ttu-id="470c9-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-266">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-267">assignmentState</span></span>|<span data-ttu-id="470c9-268">String</span><span class="sxs-lookup"><span data-stu-id="470c9-268">String</span></span>|<span data-ttu-id="470c9-269">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-269">Yes</span></span>| <span data-ttu-id="470c9-270">Aktiv</span><span class="sxs-lookup"><span data-stu-id="470c9-270">Active</span></span>|
|<span data-ttu-id="470c9-271">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-271">type</span></span>|<span data-ttu-id="470c9-272">String</span><span class="sxs-lookup"><span data-stu-id="470c9-272">String</span></span>|<span data-ttu-id="470c9-273">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-273">Yes</span></span>| <span data-ttu-id="470c9-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="470c9-274">UserAdd</span></span>|
|<span data-ttu-id="470c9-275">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-275">reason</span></span>|<span data-ttu-id="470c9-276">String</span><span class="sxs-lookup"><span data-stu-id="470c9-276">String</span></span>| <span data-ttu-id="470c9-277">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="470c9-277">depends on role Settings</span></span>||
|<span data-ttu-id="470c9-278">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-278">schedule</span></span>|[<span data-ttu-id="470c9-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-280">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-281">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-282">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="470c9-283">Beispiel 3</span><span class="sxs-lookup"><span data-stu-id="470c9-283">Example 3</span></span>
<span data-ttu-id="470c9-284">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="470c9-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="470c9-285">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-285">Property</span></span>     | <span data-ttu-id="470c9-286">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-286">Type</span></span>    |<span data-ttu-id="470c9-287">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-287">Required</span></span>|  <span data-ttu-id="470c9-288">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-289">resourceId</span></span>|<span data-ttu-id="470c9-290">String</span><span class="sxs-lookup"><span data-stu-id="470c9-290">String</span></span>|<span data-ttu-id="470c9-291">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-291">Yes</span></span>|<span data-ttu-id="470c9-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-292">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-293">roleDefinitionId</span></span>|<span data-ttu-id="470c9-294">String</span><span class="sxs-lookup"><span data-stu-id="470c9-294">String</span></span>|<span data-ttu-id="470c9-295">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-295">Yes</span></span>|<span data-ttu-id="470c9-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-297">subjectId</span></span>|<span data-ttu-id="470c9-298">String</span><span class="sxs-lookup"><span data-stu-id="470c9-298">String</span></span>|<span data-ttu-id="470c9-299">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-299">Yes</span></span>|<span data-ttu-id="470c9-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-300">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-301">assignmentState</span></span>|<span data-ttu-id="470c9-302">String</span><span class="sxs-lookup"><span data-stu-id="470c9-302">String</span></span>|<span data-ttu-id="470c9-303">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-303">Yes</span></span>| <span data-ttu-id="470c9-304">Aktiv</span><span class="sxs-lookup"><span data-stu-id="470c9-304">Active</span></span>|
|<span data-ttu-id="470c9-305">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-305">type</span></span>|<span data-ttu-id="470c9-306">String</span><span class="sxs-lookup"><span data-stu-id="470c9-306">String</span></span>|<span data-ttu-id="470c9-307">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-307">Yes</span></span>| <span data-ttu-id="470c9-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="470c9-308">UserRemove</span></span>|
|<span data-ttu-id="470c9-309">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-309">reason</span></span>|<span data-ttu-id="470c9-310">String</span><span class="sxs-lookup"><span data-stu-id="470c9-310">String</span></span>| <span data-ttu-id="470c9-311">Nein</span><span class="sxs-lookup"><span data-stu-id="470c9-311">No</span></span>||
|<span data-ttu-id="470c9-312">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-312">schedule</span></span>|[<span data-ttu-id="470c9-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-314">Nein</span><span class="sxs-lookup"><span data-stu-id="470c9-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-315">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-316">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-316">Response</span></span>
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
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="470c9-317">Beispiel 4</span><span class="sxs-lookup"><span data-stu-id="470c9-317">Example 4</span></span>
<span data-ttu-id="470c9-318">In diesem Beispiel Entfernen von Administratoren die nawu@fimdev.net Benutzer aus der Rolle Leser Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="470c9-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="470c9-319">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="470c9-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="470c9-320">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-320">Property</span></span>     | <span data-ttu-id="470c9-321">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-321">Type</span></span>    |<span data-ttu-id="470c9-322">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-322">Required</span></span>|  <span data-ttu-id="470c9-323">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-324">resourceId</span></span>|<span data-ttu-id="470c9-325">String</span><span class="sxs-lookup"><span data-stu-id="470c9-325">String</span></span>|<span data-ttu-id="470c9-326">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-326">Yes</span></span>|<span data-ttu-id="470c9-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-327">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-328">roleDefinitionId</span></span>|<span data-ttu-id="470c9-329">String</span><span class="sxs-lookup"><span data-stu-id="470c9-329">String</span></span>|<span data-ttu-id="470c9-330">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-330">Yes</span></span>|<span data-ttu-id="470c9-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-332">subjectId</span></span>|<span data-ttu-id="470c9-333">String</span><span class="sxs-lookup"><span data-stu-id="470c9-333">String</span></span>|<span data-ttu-id="470c9-334">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-334">Yes</span></span>|<span data-ttu-id="470c9-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-335">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-336">assignmentState</span></span>|<span data-ttu-id="470c9-337">String</span><span class="sxs-lookup"><span data-stu-id="470c9-337">String</span></span>|<span data-ttu-id="470c9-338">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-338">Yes</span></span>| <span data-ttu-id="470c9-339">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="470c9-339">Eligible / Active</span></span>|
|<span data-ttu-id="470c9-340">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-340">type</span></span>|<span data-ttu-id="470c9-341">String</span><span class="sxs-lookup"><span data-stu-id="470c9-341">String</span></span>|<span data-ttu-id="470c9-342">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-342">Yes</span></span>| <span data-ttu-id="470c9-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="470c9-343">AdminRemove</span></span>|
|<span data-ttu-id="470c9-344">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-344">reason</span></span>|<span data-ttu-id="470c9-345">String</span><span class="sxs-lookup"><span data-stu-id="470c9-345">String</span></span>| <span data-ttu-id="470c9-346">Nein</span><span class="sxs-lookup"><span data-stu-id="470c9-346">No</span></span>||
|<span data-ttu-id="470c9-347">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-347">schedule</span></span>|[<span data-ttu-id="470c9-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-349">Nein</span><span class="sxs-lookup"><span data-stu-id="470c9-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-350">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-351">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-351">Response</span></span>
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
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="470c9-352">Beispiel 5</span><span class="sxs-lookup"><span data-stu-id="470c9-352">Example 5</span></span>
<span data-ttu-id="470c9-353">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="470c9-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="470c9-354">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="470c9-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="470c9-355">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-355">Property</span></span>     | <span data-ttu-id="470c9-356">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-356">Type</span></span>    |<span data-ttu-id="470c9-357">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-357">Required</span></span>|  <span data-ttu-id="470c9-358">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-359">resourceId</span></span>|<span data-ttu-id="470c9-360">String</span><span class="sxs-lookup"><span data-stu-id="470c9-360">String</span></span>|<span data-ttu-id="470c9-361">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-361">Yes</span></span>|<span data-ttu-id="470c9-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-362">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-363">roleDefinitionId</span></span>|<span data-ttu-id="470c9-364">String</span><span class="sxs-lookup"><span data-stu-id="470c9-364">String</span></span>|<span data-ttu-id="470c9-365">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-365">Yes</span></span>|<span data-ttu-id="470c9-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-367">subjectId</span></span>|<span data-ttu-id="470c9-368">String</span><span class="sxs-lookup"><span data-stu-id="470c9-368">String</span></span>|<span data-ttu-id="470c9-369">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-369">Yes</span></span>|<span data-ttu-id="470c9-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-370">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-371">assignmentState</span></span>|<span data-ttu-id="470c9-372">String</span><span class="sxs-lookup"><span data-stu-id="470c9-372">String</span></span>|<span data-ttu-id="470c9-373">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-373">Yes</span></span>| <span data-ttu-id="470c9-374">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="470c9-374">Eligible / Active</span></span>|
|<span data-ttu-id="470c9-375">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-375">type</span></span>|<span data-ttu-id="470c9-376">String</span><span class="sxs-lookup"><span data-stu-id="470c9-376">String</span></span>|<span data-ttu-id="470c9-377">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-377">Yes</span></span>| <span data-ttu-id="470c9-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="470c9-378">AdminUpdate</span></span>|
|<span data-ttu-id="470c9-379">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-379">reason</span></span>|<span data-ttu-id="470c9-380">String</span><span class="sxs-lookup"><span data-stu-id="470c9-380">String</span></span>| <span data-ttu-id="470c9-381">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="470c9-381">depends on roleSettings</span></span>||
|<span data-ttu-id="470c9-382">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-382">schedule</span></span>|[<span data-ttu-id="470c9-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-384">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-385">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-386">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="470c9-387">Beispiel 6</span><span class="sxs-lookup"><span data-stu-id="470c9-387">Example 6</span></span>
<span data-ttu-id="470c9-388">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="470c9-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="470c9-389">**Hinweis:** In Additon die Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="470c9-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="470c9-390">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="470c9-390">Property</span></span>     | <span data-ttu-id="470c9-391">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-391">Type</span></span>    |<span data-ttu-id="470c9-392">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="470c9-392">Required</span></span>|  <span data-ttu-id="470c9-393">Wert</span><span class="sxs-lookup"><span data-stu-id="470c9-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="470c9-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="470c9-394">resourceId</span></span>|<span data-ttu-id="470c9-395">String</span><span class="sxs-lookup"><span data-stu-id="470c9-395">String</span></span>|<span data-ttu-id="470c9-396">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-396">Yes</span></span>|<span data-ttu-id="470c9-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="470c9-397">\<resourceId\></span></span>|
|<span data-ttu-id="470c9-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="470c9-398">roleDefinitionId</span></span>|<span data-ttu-id="470c9-399">String</span><span class="sxs-lookup"><span data-stu-id="470c9-399">String</span></span>|<span data-ttu-id="470c9-400">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-400">Yes</span></span>|<span data-ttu-id="470c9-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="470c9-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="470c9-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="470c9-402">subjectId</span></span>|<span data-ttu-id="470c9-403">String</span><span class="sxs-lookup"><span data-stu-id="470c9-403">String</span></span>|<span data-ttu-id="470c9-404">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-404">Yes</span></span>|<span data-ttu-id="470c9-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="470c9-405">\<subjectId\></span></span>|
|<span data-ttu-id="470c9-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="470c9-406">assignmentState</span></span>|<span data-ttu-id="470c9-407">String</span><span class="sxs-lookup"><span data-stu-id="470c9-407">String</span></span>|<span data-ttu-id="470c9-408">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-408">Yes</span></span>| <span data-ttu-id="470c9-409">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="470c9-409">Eligible / Active</span></span> |
|<span data-ttu-id="470c9-410">Typ</span><span class="sxs-lookup"><span data-stu-id="470c9-410">type</span></span>|<span data-ttu-id="470c9-411">String</span><span class="sxs-lookup"><span data-stu-id="470c9-411">String</span></span>|<span data-ttu-id="470c9-412">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-412">Yes</span></span>| <span data-ttu-id="470c9-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="470c9-413">AdminExtend</span></span>|
|<span data-ttu-id="470c9-414">Grund</span><span class="sxs-lookup"><span data-stu-id="470c9-414">reason</span></span>|<span data-ttu-id="470c9-415">String</span><span class="sxs-lookup"><span data-stu-id="470c9-415">String</span></span>| <span data-ttu-id="470c9-416">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="470c9-416">depends on roleSettings</span></span>||
|<span data-ttu-id="470c9-417">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="470c9-417">schedule</span></span>|[<span data-ttu-id="470c9-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="470c9-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="470c9-419">Ja</span><span class="sxs-lookup"><span data-stu-id="470c9-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="470c9-420">Anforderung</span><span class="sxs-lookup"><span data-stu-id="470c9-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="470c9-421">Antwort</span><span class="sxs-lookup"><span data-stu-id="470c9-421">Response</span></span>
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
