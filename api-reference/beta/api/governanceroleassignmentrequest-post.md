---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
localization_priority: Normal
ms.openlocfilehash: 0fc8d96585daf63f53bc6b33985a289e8f810d6b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572367"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="f0627-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0627-105">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="f0627-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="f0627-106">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="f0627-106">The following table lists the operations.</span></span>

| <span data-ttu-id="f0627-107">Vorgang</span><span class="sxs-lookup"><span data-stu-id="f0627-107">Operation</span></span>       | <span data-ttu-id="f0627-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="f0627-109">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-109">Assign a role assignment</span></span>| <span data-ttu-id="f0627-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="f0627-110">AdminAdd</span></span> |
| <span data-ttu-id="f0627-111">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="f0627-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="f0627-112">UserAdd</span></span> | 
| <span data-ttu-id="f0627-113">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="f0627-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="f0627-114">UserRemove</span></span> | 
| <span data-ttu-id="f0627-115">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-115">Remove a role assignment</span></span>| <span data-ttu-id="f0627-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="f0627-116">AdminRemove</span></span> |
| <span data-ttu-id="f0627-117">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-117">Update a role assignment</span></span>| <span data-ttu-id="f0627-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="f0627-118">AdminUpdate</span></span> |
| <span data-ttu-id="f0627-119">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="f0627-119">Request to extend my role assignment</span></span>| <span data-ttu-id="f0627-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="f0627-120">UserExtend</span></span> | 
| <span data-ttu-id="f0627-121">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-121">Extend a role assignment</span></span>| <span data-ttu-id="f0627-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="f0627-122">AdminExtend</span></span> | 
| <span data-ttu-id="f0627-123">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="f0627-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="f0627-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="f0627-124">UserRenew</span></span> | 
| <span data-ttu-id="f0627-125">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="f0627-125">Renew an expired role assignment</span></span>| <span data-ttu-id="f0627-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="f0627-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="f0627-127">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0627-127">Permissions</span></span>
<span data-ttu-id="f0627-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0627-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0627-130">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0627-130">Permission type</span></span>      | <span data-ttu-id="f0627-131">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0627-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0627-132">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0627-132">Delegated (work or school account)</span></span> | <span data-ttu-id="f0627-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f0627-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f0627-134">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0627-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0627-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0627-135">Not supported.</span></span>    |
|<span data-ttu-id="f0627-136">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0627-136">Application</span></span> | <span data-ttu-id="f0627-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f0627-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0627-138">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="f0627-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0627-139">Request headers</span></span>
| <span data-ttu-id="f0627-140">Name</span><span class="sxs-lookup"><span data-stu-id="f0627-140">Name</span></span>       | <span data-ttu-id="f0627-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0627-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0627-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0627-142">Authorization</span></span>  | <span data-ttu-id="f0627-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f0627-143">Bearer {code}</span></span>|
| <span data-ttu-id="f0627-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="f0627-144">Content-type</span></span>  | <span data-ttu-id="f0627-145">application/json</span><span class="sxs-lookup"><span data-stu-id="f0627-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0627-146">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0627-146">Request body</span></span>
<span data-ttu-id="f0627-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0627-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="f0627-148">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-148">Property</span></span>     | <span data-ttu-id="f0627-149">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-149">Type</span></span>    |<span data-ttu-id="f0627-150">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-150">Required</span></span>|  <span data-ttu-id="f0627-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0627-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-152">resourceId</span></span>|<span data-ttu-id="f0627-153">String</span><span class="sxs-lookup"><span data-stu-id="f0627-153">String</span></span>|<span data-ttu-id="f0627-154">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-154">Yes</span></span>|<span data-ttu-id="f0627-155">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0627-155">The ID of the resource.</span></span>|
|<span data-ttu-id="f0627-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-156">roleDefinitionId</span></span>|<span data-ttu-id="f0627-157">String</span><span class="sxs-lookup"><span data-stu-id="f0627-157">String</span></span>|<span data-ttu-id="f0627-158">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-158">Yes</span></span>|<span data-ttu-id="f0627-159">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="f0627-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="f0627-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-160">subjectId</span></span>|<span data-ttu-id="f0627-161">String</span><span class="sxs-lookup"><span data-stu-id="f0627-161">String</span></span>|<span data-ttu-id="f0627-162">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-162">Yes</span></span>|<span data-ttu-id="f0627-163">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="f0627-163">The ID of the subject.</span></span>|
|<span data-ttu-id="f0627-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-164">assignmentState</span></span>|<span data-ttu-id="f0627-165">String</span><span class="sxs-lookup"><span data-stu-id="f0627-165">String</span></span>|<span data-ttu-id="f0627-166">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-166">Yes</span></span>|<span data-ttu-id="f0627-167">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="f0627-167">The state of assignment.</span></span> <span data-ttu-id="f0627-168">Der Wert kann sein ``Eligible`` und ``Active``.</span><span class="sxs-lookup"><span data-stu-id="f0627-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="f0627-169">type</span><span class="sxs-lookup"><span data-stu-id="f0627-169">type</span></span>|<span data-ttu-id="f0627-170">String</span><span class="sxs-lookup"><span data-stu-id="f0627-170">String</span></span>|<span data-ttu-id="f0627-171">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-171">Yes</span></span>|<span data-ttu-id="f0627-172">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="f0627-172">The request type.</span></span> <span data-ttu-id="f0627-173">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="f0627-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="f0627-174">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-174">reason</span></span>|<span data-ttu-id="f0627-175">String</span><span class="sxs-lookup"><span data-stu-id="f0627-175">String</span></span>| |<span data-ttu-id="f0627-176">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="f0627-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="f0627-177">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-177">schedule</span></span>|[<span data-ttu-id="f0627-178">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-178">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="f0627-179">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f0627-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="f0627-180">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f0627-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="f0627-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-181">Response</span></span>
<span data-ttu-id="f0627-182">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f0627-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="f0627-183">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="f0627-183">Error codes</span></span>
<span data-ttu-id="f0627-184">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="f0627-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f0627-185">Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.</span><span class="sxs-lookup"><span data-stu-id="f0627-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="f0627-186">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="f0627-186">Error code</span></span>     | <span data-ttu-id="f0627-187">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="f0627-187">Error message</span></span>              | <span data-ttu-id="f0627-188">Details</span><span class="sxs-lookup"><span data-stu-id="f0627-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="f0627-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-189">400 BadRequest</span></span> | <span data-ttu-id="f0627-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="f0627-190">RoleNotFound</span></span>    | <span data-ttu-id="f0627-191">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="f0627-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="f0627-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-192">400 BadRequest</span></span> | <span data-ttu-id="f0627-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="f0627-193">ResourceIsLocked</span></span>    | <span data-ttu-id="f0627-194">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f0627-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="f0627-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-195">400 BadRequest</span></span> | <span data-ttu-id="f0627-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="f0627-196">SubjectNotFound</span></span>    | <span data-ttu-id="f0627-197">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="f0627-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="f0627-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-198">400 BadRequest</span></span> | <span data-ttu-id="f0627-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="f0627-200">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="f0627-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="f0627-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-201">400 BadRequest</span></span> | <span data-ttu-id="f0627-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="f0627-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="f0627-203">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f0627-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="f0627-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-204">400 BadRequest</span></span> | <span data-ttu-id="f0627-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="f0627-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="f0627-206">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="f0627-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="f0627-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f0627-207">400 BadRequest</span></span> | <span data-ttu-id="f0627-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="f0627-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="f0627-209">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f0627-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="f0627-210">Beispiele</span><span class="sxs-lookup"><span data-stu-id="f0627-210">Examples</span></span>
<span data-ttu-id="f0627-211">Die folgenden Beispiele zeigen, wie diese API verwendet.</span><span class="sxs-lookup"><span data-stu-id="f0627-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="f0627-212">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="f0627-212">Example 1</span></span>
<span data-ttu-id="f0627-213">In diesem Beispiel weisen Sie Administratoren Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="f0627-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="f0627-214">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0627-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="f0627-215">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-215">Property</span></span>     | <span data-ttu-id="f0627-216">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-216">Type</span></span>    |<span data-ttu-id="f0627-217">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-217">Required</span></span>|  <span data-ttu-id="f0627-218">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-219">resourceId</span></span>|<span data-ttu-id="f0627-220">String</span><span class="sxs-lookup"><span data-stu-id="f0627-220">String</span></span>|<span data-ttu-id="f0627-221">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-221">Yes</span></span>|<span data-ttu-id="f0627-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-222">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-223">roleDefinitionId</span></span>|<span data-ttu-id="f0627-224">String</span><span class="sxs-lookup"><span data-stu-id="f0627-224">String</span></span>|<span data-ttu-id="f0627-225">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-225">Yes</span></span>|<span data-ttu-id="f0627-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-227">subjectId</span></span>|<span data-ttu-id="f0627-228">String</span><span class="sxs-lookup"><span data-stu-id="f0627-228">String</span></span>|<span data-ttu-id="f0627-229">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-229">Yes</span></span>|<span data-ttu-id="f0627-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-230">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-231">assignmentState</span></span>|<span data-ttu-id="f0627-232">String</span><span class="sxs-lookup"><span data-stu-id="f0627-232">String</span></span>|<span data-ttu-id="f0627-233">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-233">Yes</span></span>| <span data-ttu-id="f0627-234">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="f0627-234">Eligible / Active</span></span>|
|<span data-ttu-id="f0627-235">type</span><span class="sxs-lookup"><span data-stu-id="f0627-235">type</span></span>|<span data-ttu-id="f0627-236">String</span><span class="sxs-lookup"><span data-stu-id="f0627-236">String</span></span>|<span data-ttu-id="f0627-237">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-237">Yes</span></span>| <span data-ttu-id="f0627-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="f0627-238">AdminAdd</span></span>|
|<span data-ttu-id="f0627-239">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-239">reason</span></span>|<span data-ttu-id="f0627-240">String</span><span class="sxs-lookup"><span data-stu-id="f0627-240">String</span></span>| <span data-ttu-id="f0627-241">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="f0627-241">depends on role Settings</span></span>||
|<span data-ttu-id="f0627-242">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-242">schedule</span></span>|[<span data-ttu-id="f0627-243">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-243">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-244">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="f0627-247">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="f0627-247">Example 2</span></span>
<span data-ttu-id="f0627-248">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f0627-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="f0627-249">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-249">Property</span></span>     | <span data-ttu-id="f0627-250">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-250">Type</span></span>    |<span data-ttu-id="f0627-251">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-251">Required</span></span>|  <span data-ttu-id="f0627-252">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-253">resourceId</span></span>|<span data-ttu-id="f0627-254">String</span><span class="sxs-lookup"><span data-stu-id="f0627-254">String</span></span>|<span data-ttu-id="f0627-255">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-255">Yes</span></span>|<span data-ttu-id="f0627-256">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-256">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-257">roleDefinitionId</span></span>|<span data-ttu-id="f0627-258">String</span><span class="sxs-lookup"><span data-stu-id="f0627-258">String</span></span>|<span data-ttu-id="f0627-259">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-259">Yes</span></span>|<span data-ttu-id="f0627-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-261">subjectId</span></span>|<span data-ttu-id="f0627-262">String</span><span class="sxs-lookup"><span data-stu-id="f0627-262">String</span></span>|<span data-ttu-id="f0627-263">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-263">Yes</span></span>|<span data-ttu-id="f0627-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-264">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-265">assignmentState</span></span>|<span data-ttu-id="f0627-266">String</span><span class="sxs-lookup"><span data-stu-id="f0627-266">String</span></span>|<span data-ttu-id="f0627-267">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-267">Yes</span></span>| <span data-ttu-id="f0627-268">Aktiv</span><span class="sxs-lookup"><span data-stu-id="f0627-268">Active</span></span>|
|<span data-ttu-id="f0627-269">type</span><span class="sxs-lookup"><span data-stu-id="f0627-269">type</span></span>|<span data-ttu-id="f0627-270">String</span><span class="sxs-lookup"><span data-stu-id="f0627-270">String</span></span>|<span data-ttu-id="f0627-271">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-271">Yes</span></span>| <span data-ttu-id="f0627-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="f0627-272">UserAdd</span></span>|
|<span data-ttu-id="f0627-273">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-273">reason</span></span>|<span data-ttu-id="f0627-274">String</span><span class="sxs-lookup"><span data-stu-id="f0627-274">String</span></span>| <span data-ttu-id="f0627-275">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="f0627-275">depends on role Settings</span></span>||
|<span data-ttu-id="f0627-276">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-276">schedule</span></span>|[<span data-ttu-id="f0627-277">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-277">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-278">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-279">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="f0627-281">Beispiel 3</span><span class="sxs-lookup"><span data-stu-id="f0627-281">Example 3</span></span>
<span data-ttu-id="f0627-282">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="f0627-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="f0627-283">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-283">Property</span></span>     | <span data-ttu-id="f0627-284">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-284">Type</span></span>    |<span data-ttu-id="f0627-285">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-285">Required</span></span>|  <span data-ttu-id="f0627-286">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-287">resourceId</span></span>|<span data-ttu-id="f0627-288">String</span><span class="sxs-lookup"><span data-stu-id="f0627-288">String</span></span>|<span data-ttu-id="f0627-289">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-289">Yes</span></span>|<span data-ttu-id="f0627-290">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-290">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-291">roleDefinitionId</span></span>|<span data-ttu-id="f0627-292">String</span><span class="sxs-lookup"><span data-stu-id="f0627-292">String</span></span>|<span data-ttu-id="f0627-293">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-293">Yes</span></span>|<span data-ttu-id="f0627-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-295">subjectId</span></span>|<span data-ttu-id="f0627-296">String</span><span class="sxs-lookup"><span data-stu-id="f0627-296">String</span></span>|<span data-ttu-id="f0627-297">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-297">Yes</span></span>|<span data-ttu-id="f0627-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-298">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-299">assignmentState</span></span>|<span data-ttu-id="f0627-300">String</span><span class="sxs-lookup"><span data-stu-id="f0627-300">String</span></span>|<span data-ttu-id="f0627-301">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-301">Yes</span></span>| <span data-ttu-id="f0627-302">Aktiv</span><span class="sxs-lookup"><span data-stu-id="f0627-302">Active</span></span>|
|<span data-ttu-id="f0627-303">type</span><span class="sxs-lookup"><span data-stu-id="f0627-303">type</span></span>|<span data-ttu-id="f0627-304">String</span><span class="sxs-lookup"><span data-stu-id="f0627-304">String</span></span>|<span data-ttu-id="f0627-305">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-305">Yes</span></span>| <span data-ttu-id="f0627-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="f0627-306">UserRemove</span></span>|
|<span data-ttu-id="f0627-307">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-307">reason</span></span>|<span data-ttu-id="f0627-308">String</span><span class="sxs-lookup"><span data-stu-id="f0627-308">String</span></span>| <span data-ttu-id="f0627-309">Nein</span><span class="sxs-lookup"><span data-stu-id="f0627-309">No</span></span>||
|<span data-ttu-id="f0627-310">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-310">schedule</span></span>|[<span data-ttu-id="f0627-311">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-311">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-312">No</span><span class="sxs-lookup"><span data-stu-id="f0627-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-313">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-314">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="f0627-315">Beispiel 4</span><span class="sxs-lookup"><span data-stu-id="f0627-315">Example 4</span></span>
<span data-ttu-id="f0627-316">In diesem Beispiel Entfernen von Administratoren die nawu@fimdev.net Benutzer aus der Rolle Leser Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="f0627-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="f0627-317">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0627-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="f0627-318">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-318">Property</span></span>     | <span data-ttu-id="f0627-319">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-319">Type</span></span>    |<span data-ttu-id="f0627-320">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-320">Required</span></span>|  <span data-ttu-id="f0627-321">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-322">resourceId</span></span>|<span data-ttu-id="f0627-323">String</span><span class="sxs-lookup"><span data-stu-id="f0627-323">String</span></span>|<span data-ttu-id="f0627-324">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-324">Yes</span></span>|<span data-ttu-id="f0627-325">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-325">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-326">roleDefinitionId</span></span>|<span data-ttu-id="f0627-327">String</span><span class="sxs-lookup"><span data-stu-id="f0627-327">String</span></span>|<span data-ttu-id="f0627-328">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-328">Yes</span></span>|<span data-ttu-id="f0627-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-330">subjectId</span></span>|<span data-ttu-id="f0627-331">String</span><span class="sxs-lookup"><span data-stu-id="f0627-331">String</span></span>|<span data-ttu-id="f0627-332">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-332">Yes</span></span>|<span data-ttu-id="f0627-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-333">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-334">assignmentState</span></span>|<span data-ttu-id="f0627-335">String</span><span class="sxs-lookup"><span data-stu-id="f0627-335">String</span></span>|<span data-ttu-id="f0627-336">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-336">Yes</span></span>| <span data-ttu-id="f0627-337">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="f0627-337">Eligible / Active</span></span>|
|<span data-ttu-id="f0627-338">type</span><span class="sxs-lookup"><span data-stu-id="f0627-338">type</span></span>|<span data-ttu-id="f0627-339">String</span><span class="sxs-lookup"><span data-stu-id="f0627-339">String</span></span>|<span data-ttu-id="f0627-340">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-340">Yes</span></span>| <span data-ttu-id="f0627-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="f0627-341">AdminRemove</span></span>|
|<span data-ttu-id="f0627-342">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-342">reason</span></span>|<span data-ttu-id="f0627-343">String</span><span class="sxs-lookup"><span data-stu-id="f0627-343">String</span></span>| <span data-ttu-id="f0627-344">Nein</span><span class="sxs-lookup"><span data-stu-id="f0627-344">No</span></span>||
|<span data-ttu-id="f0627-345">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-345">schedule</span></span>|[<span data-ttu-id="f0627-346">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-346">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-347">No</span><span class="sxs-lookup"><span data-stu-id="f0627-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-348">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-349">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="f0627-350">Beispiel 5</span><span class="sxs-lookup"><span data-stu-id="f0627-350">Example 5</span></span>
<span data-ttu-id="f0627-351">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="f0627-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="f0627-352">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0627-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="f0627-353">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-353">Property</span></span>     | <span data-ttu-id="f0627-354">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-354">Type</span></span>    |<span data-ttu-id="f0627-355">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-355">Required</span></span>|  <span data-ttu-id="f0627-356">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-357">resourceId</span></span>|<span data-ttu-id="f0627-358">String</span><span class="sxs-lookup"><span data-stu-id="f0627-358">String</span></span>|<span data-ttu-id="f0627-359">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-359">Yes</span></span>|<span data-ttu-id="f0627-360">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-360">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-361">roleDefinitionId</span></span>|<span data-ttu-id="f0627-362">String</span><span class="sxs-lookup"><span data-stu-id="f0627-362">String</span></span>|<span data-ttu-id="f0627-363">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-363">Yes</span></span>|<span data-ttu-id="f0627-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-365">subjectId</span></span>|<span data-ttu-id="f0627-366">String</span><span class="sxs-lookup"><span data-stu-id="f0627-366">String</span></span>|<span data-ttu-id="f0627-367">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-367">Yes</span></span>|<span data-ttu-id="f0627-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-368">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-369">assignmentState</span></span>|<span data-ttu-id="f0627-370">String</span><span class="sxs-lookup"><span data-stu-id="f0627-370">String</span></span>|<span data-ttu-id="f0627-371">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-371">Yes</span></span>| <span data-ttu-id="f0627-372">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="f0627-372">Eligible / Active</span></span>|
|<span data-ttu-id="f0627-373">type</span><span class="sxs-lookup"><span data-stu-id="f0627-373">type</span></span>|<span data-ttu-id="f0627-374">String</span><span class="sxs-lookup"><span data-stu-id="f0627-374">String</span></span>|<span data-ttu-id="f0627-375">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-375">Yes</span></span>| <span data-ttu-id="f0627-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="f0627-376">AdminUpdate</span></span>|
|<span data-ttu-id="f0627-377">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-377">reason</span></span>|<span data-ttu-id="f0627-378">String</span><span class="sxs-lookup"><span data-stu-id="f0627-378">String</span></span>| <span data-ttu-id="f0627-379">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="f0627-379">depends on roleSettings</span></span>||
|<span data-ttu-id="f0627-380">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-380">schedule</span></span>|[<span data-ttu-id="f0627-381">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-381">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-382">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-383">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-384">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="f0627-385">Beispiel 6</span><span class="sxs-lookup"><span data-stu-id="f0627-385">Example 6</span></span>
<span data-ttu-id="f0627-386">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="f0627-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="f0627-387">**Hinweis:** In Additon die Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0627-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="f0627-388">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0627-388">Property</span></span>     | <span data-ttu-id="f0627-389">Typ</span><span class="sxs-lookup"><span data-stu-id="f0627-389">Type</span></span>    |<span data-ttu-id="f0627-390">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0627-390">Required</span></span>|  <span data-ttu-id="f0627-391">Wert</span><span class="sxs-lookup"><span data-stu-id="f0627-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f0627-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0627-392">resourceId</span></span>|<span data-ttu-id="f0627-393">String</span><span class="sxs-lookup"><span data-stu-id="f0627-393">String</span></span>|<span data-ttu-id="f0627-394">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-394">Yes</span></span>|<span data-ttu-id="f0627-395">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f0627-395">\<resourceId\></span></span>|
|<span data-ttu-id="f0627-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f0627-396">roleDefinitionId</span></span>|<span data-ttu-id="f0627-397">String</span><span class="sxs-lookup"><span data-stu-id="f0627-397">String</span></span>|<span data-ttu-id="f0627-398">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-398">Yes</span></span>|<span data-ttu-id="f0627-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f0627-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="f0627-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="f0627-400">subjectId</span></span>|<span data-ttu-id="f0627-401">String</span><span class="sxs-lookup"><span data-stu-id="f0627-401">String</span></span>|<span data-ttu-id="f0627-402">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-402">Yes</span></span>|<span data-ttu-id="f0627-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="f0627-403">\<subjectId\></span></span>|
|<span data-ttu-id="f0627-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f0627-404">assignmentState</span></span>|<span data-ttu-id="f0627-405">String</span><span class="sxs-lookup"><span data-stu-id="f0627-405">String</span></span>|<span data-ttu-id="f0627-406">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-406">Yes</span></span>| <span data-ttu-id="f0627-407">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="f0627-407">Eligible / Active</span></span> |
|<span data-ttu-id="f0627-408">type</span><span class="sxs-lookup"><span data-stu-id="f0627-408">type</span></span>|<span data-ttu-id="f0627-409">String</span><span class="sxs-lookup"><span data-stu-id="f0627-409">String</span></span>|<span data-ttu-id="f0627-410">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-410">Yes</span></span>| <span data-ttu-id="f0627-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="f0627-411">AdminExtend</span></span>|
|<span data-ttu-id="f0627-412">Grund</span><span class="sxs-lookup"><span data-stu-id="f0627-412">reason</span></span>|<span data-ttu-id="f0627-413">String</span><span class="sxs-lookup"><span data-stu-id="f0627-413">String</span></span>| <span data-ttu-id="f0627-414">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="f0627-414">depends on roleSettings</span></span>||
|<span data-ttu-id="f0627-415">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="f0627-415">schedule</span></span>|[<span data-ttu-id="f0627-416">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f0627-416">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f0627-417">Ja</span><span class="sxs-lookup"><span data-stu-id="f0627-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="f0627-418">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0627-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0627-419">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0627-419">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
