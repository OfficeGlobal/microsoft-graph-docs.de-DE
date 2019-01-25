---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523239"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="2a459-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a459-105">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="2a459-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="2a459-106">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="2a459-106">The following table lists the operations.</span></span>

| <span data-ttu-id="2a459-107">Vorgang</span><span class="sxs-lookup"><span data-stu-id="2a459-107">Operation</span></span>       | <span data-ttu-id="2a459-108">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="2a459-109">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-109">Assign a role assignment</span></span>| <span data-ttu-id="2a459-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="2a459-110">AdminAdd</span></span> |
| <span data-ttu-id="2a459-111">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="2a459-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="2a459-112">UserAdd</span></span> | 
| <span data-ttu-id="2a459-113">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="2a459-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="2a459-114">UserRemove</span></span> | 
| <span data-ttu-id="2a459-115">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-115">Remove a role assignment</span></span>| <span data-ttu-id="2a459-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="2a459-116">AdminRemove</span></span> |
| <span data-ttu-id="2a459-117">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-117">Update a role assignment</span></span>| <span data-ttu-id="2a459-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="2a459-118">AdminUpdate</span></span> |
| <span data-ttu-id="2a459-119">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="2a459-119">Request to extend my role assignment</span></span>| <span data-ttu-id="2a459-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="2a459-120">UserExtend</span></span> | 
| <span data-ttu-id="2a459-121">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-121">Extend a role assignment</span></span>| <span data-ttu-id="2a459-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="2a459-122">AdminExtend</span></span> | 
| <span data-ttu-id="2a459-123">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="2a459-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="2a459-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="2a459-124">UserRenew</span></span> | 
| <span data-ttu-id="2a459-125">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="2a459-125">Renew an expired role assignment</span></span>| <span data-ttu-id="2a459-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="2a459-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="2a459-127">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a459-127">Permissions</span></span>
<span data-ttu-id="2a459-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a459-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a459-130">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a459-130">Permission type</span></span>      | <span data-ttu-id="2a459-131">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a459-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a459-132">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a459-132">Delegated (work or school account)</span></span> | <span data-ttu-id="2a459-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2a459-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2a459-134">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a459-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a459-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a459-135">Not supported.</span></span>    |
|<span data-ttu-id="2a459-136">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a459-136">Application</span></span> | <span data-ttu-id="2a459-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2a459-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a459-138">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2a459-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a459-139">Request headers</span></span>
| <span data-ttu-id="2a459-140">Name</span><span class="sxs-lookup"><span data-stu-id="2a459-140">Name</span></span>       | <span data-ttu-id="2a459-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a459-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a459-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a459-142">Authorization</span></span>  | <span data-ttu-id="2a459-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2a459-143">Bearer {code}</span></span>|
| <span data-ttu-id="2a459-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="2a459-144">Content-type</span></span>  | <span data-ttu-id="2a459-145">application/json</span><span class="sxs-lookup"><span data-stu-id="2a459-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a459-146">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a459-146">Request body</span></span>
<span data-ttu-id="2a459-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a459-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="2a459-148">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-148">Property</span></span>     | <span data-ttu-id="2a459-149">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-149">Type</span></span>    |<span data-ttu-id="2a459-150">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-150">Required</span></span>|  <span data-ttu-id="2a459-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a459-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-152">resourceId</span></span>|<span data-ttu-id="2a459-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-153">String</span></span>|<span data-ttu-id="2a459-154">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-154">Yes</span></span>|<span data-ttu-id="2a459-155">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a459-155">The ID of the resource.</span></span>|
|<span data-ttu-id="2a459-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-156">roleDefinitionId</span></span>|<span data-ttu-id="2a459-157">String</span><span class="sxs-lookup"><span data-stu-id="2a459-157">String</span></span>|<span data-ttu-id="2a459-158">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-158">Yes</span></span>|<span data-ttu-id="2a459-159">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="2a459-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="2a459-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-160">subjectId</span></span>|<span data-ttu-id="2a459-161">String</span><span class="sxs-lookup"><span data-stu-id="2a459-161">String</span></span>|<span data-ttu-id="2a459-162">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-162">Yes</span></span>|<span data-ttu-id="2a459-163">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="2a459-163">The ID of the subject.</span></span>|
|<span data-ttu-id="2a459-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-164">assignmentState</span></span>|<span data-ttu-id="2a459-165">String</span><span class="sxs-lookup"><span data-stu-id="2a459-165">String</span></span>|<span data-ttu-id="2a459-166">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-166">Yes</span></span>|<span data-ttu-id="2a459-167">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="2a459-167">The state of assignment.</span></span> <span data-ttu-id="2a459-168">Der Wert kann sein ``Eligible`` und ``Active``.</span><span class="sxs-lookup"><span data-stu-id="2a459-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="2a459-169">type</span><span class="sxs-lookup"><span data-stu-id="2a459-169">type</span></span>|<span data-ttu-id="2a459-170">String</span><span class="sxs-lookup"><span data-stu-id="2a459-170">String</span></span>|<span data-ttu-id="2a459-171">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-171">Yes</span></span>|<span data-ttu-id="2a459-172">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="2a459-172">The request type.</span></span> <span data-ttu-id="2a459-173">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="2a459-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="2a459-174">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-174">reason</span></span>|<span data-ttu-id="2a459-175">String</span><span class="sxs-lookup"><span data-stu-id="2a459-175">String</span></span>| |<span data-ttu-id="2a459-176">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="2a459-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="2a459-177">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-177">schedule</span></span>|[<span data-ttu-id="2a459-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="2a459-179">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a459-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="2a459-180">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a459-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="2a459-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-181">Response</span></span>
<span data-ttu-id="2a459-182">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2a459-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="2a459-183">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="2a459-183">Error codes</span></span>
<span data-ttu-id="2a459-184">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="2a459-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="2a459-185">Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.</span><span class="sxs-lookup"><span data-stu-id="2a459-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="2a459-186">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="2a459-186">Error code</span></span>     | <span data-ttu-id="2a459-187">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="2a459-187">Error message</span></span>              | <span data-ttu-id="2a459-188">Details</span><span class="sxs-lookup"><span data-stu-id="2a459-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="2a459-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-189">400 BadRequest</span></span> | <span data-ttu-id="2a459-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="2a459-190">RoleNotFound</span></span>    | <span data-ttu-id="2a459-191">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="2a459-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="2a459-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-192">400 BadRequest</span></span> | <span data-ttu-id="2a459-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="2a459-193">ResourceIsLocked</span></span>    | <span data-ttu-id="2a459-194">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="2a459-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="2a459-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-195">400 BadRequest</span></span> | <span data-ttu-id="2a459-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="2a459-196">SubjectNotFound</span></span>    | <span data-ttu-id="2a459-197">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="2a459-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="2a459-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-198">400 BadRequest</span></span> | <span data-ttu-id="2a459-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="2a459-200">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="2a459-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="2a459-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-201">400 BadRequest</span></span> | <span data-ttu-id="2a459-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="2a459-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="2a459-203">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="2a459-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="2a459-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-204">400 BadRequest</span></span> | <span data-ttu-id="2a459-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="2a459-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="2a459-206">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="2a459-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="2a459-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2a459-207">400 BadRequest</span></span> | <span data-ttu-id="2a459-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="2a459-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="2a459-209">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="2a459-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="2a459-210">Beispiele</span><span class="sxs-lookup"><span data-stu-id="2a459-210">Examples</span></span>
<span data-ttu-id="2a459-211">Die folgenden Beispiele zeigen, wie diese API verwendet.</span><span class="sxs-lookup"><span data-stu-id="2a459-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="2a459-212">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="2a459-212">Example 1</span></span>
<span data-ttu-id="2a459-213">In diesem Beispiel weisen Sie Administratoren Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="2a459-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="2a459-214">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a459-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="2a459-215">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-215">Property</span></span>     | <span data-ttu-id="2a459-216">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-216">Type</span></span>    |<span data-ttu-id="2a459-217">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-217">Required</span></span>|  <span data-ttu-id="2a459-218">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-219">resourceId</span></span>|<span data-ttu-id="2a459-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-220">String</span></span>|<span data-ttu-id="2a459-221">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-221">Yes</span></span>|<span data-ttu-id="2a459-222">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-222">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-223">roleDefinitionId</span></span>|<span data-ttu-id="2a459-224">String</span><span class="sxs-lookup"><span data-stu-id="2a459-224">String</span></span>|<span data-ttu-id="2a459-225">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-225">Yes</span></span>|<span data-ttu-id="2a459-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-227">subjectId</span></span>|<span data-ttu-id="2a459-228">String</span><span class="sxs-lookup"><span data-stu-id="2a459-228">String</span></span>|<span data-ttu-id="2a459-229">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-229">Yes</span></span>|<span data-ttu-id="2a459-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-230">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-231">assignmentState</span></span>|<span data-ttu-id="2a459-232">String</span><span class="sxs-lookup"><span data-stu-id="2a459-232">String</span></span>|<span data-ttu-id="2a459-233">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-233">Yes</span></span>| <span data-ttu-id="2a459-234">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="2a459-234">Eligible / Active</span></span>|
|<span data-ttu-id="2a459-235">type</span><span class="sxs-lookup"><span data-stu-id="2a459-235">type</span></span>|<span data-ttu-id="2a459-236">String</span><span class="sxs-lookup"><span data-stu-id="2a459-236">String</span></span>|<span data-ttu-id="2a459-237">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-237">Yes</span></span>| <span data-ttu-id="2a459-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="2a459-238">AdminAdd</span></span>|
|<span data-ttu-id="2a459-239">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-239">reason</span></span>|<span data-ttu-id="2a459-240">String</span><span class="sxs-lookup"><span data-stu-id="2a459-240">String</span></span>| <span data-ttu-id="2a459-241">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2a459-241">depends on role Settings</span></span>||
|<span data-ttu-id="2a459-242">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-242">schedule</span></span>|[<span data-ttu-id="2a459-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-244">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="2a459-247">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="2a459-247">Example 2</span></span>
<span data-ttu-id="2a459-248">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2a459-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="2a459-249">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-249">Property</span></span>     | <span data-ttu-id="2a459-250">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-250">Type</span></span>    |<span data-ttu-id="2a459-251">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-251">Required</span></span>|  <span data-ttu-id="2a459-252">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-253">resourceId</span></span>|<span data-ttu-id="2a459-254">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-254">String</span></span>|<span data-ttu-id="2a459-255">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-255">Yes</span></span>|<span data-ttu-id="2a459-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-256">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-257">roleDefinitionId</span></span>|<span data-ttu-id="2a459-258">String</span><span class="sxs-lookup"><span data-stu-id="2a459-258">String</span></span>|<span data-ttu-id="2a459-259">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-259">Yes</span></span>|<span data-ttu-id="2a459-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-261">subjectId</span></span>|<span data-ttu-id="2a459-262">String</span><span class="sxs-lookup"><span data-stu-id="2a459-262">String</span></span>|<span data-ttu-id="2a459-263">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-263">Yes</span></span>|<span data-ttu-id="2a459-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-264">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-265">assignmentState</span></span>|<span data-ttu-id="2a459-266">String</span><span class="sxs-lookup"><span data-stu-id="2a459-266">String</span></span>|<span data-ttu-id="2a459-267">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-267">Yes</span></span>| <span data-ttu-id="2a459-268">Aktiv</span><span class="sxs-lookup"><span data-stu-id="2a459-268">Active</span></span>|
|<span data-ttu-id="2a459-269">type</span><span class="sxs-lookup"><span data-stu-id="2a459-269">type</span></span>|<span data-ttu-id="2a459-270">String</span><span class="sxs-lookup"><span data-stu-id="2a459-270">String</span></span>|<span data-ttu-id="2a459-271">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-271">Yes</span></span>| <span data-ttu-id="2a459-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="2a459-272">UserAdd</span></span>|
|<span data-ttu-id="2a459-273">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-273">reason</span></span>|<span data-ttu-id="2a459-274">String</span><span class="sxs-lookup"><span data-stu-id="2a459-274">String</span></span>| <span data-ttu-id="2a459-275">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2a459-275">depends on role Settings</span></span>||
|<span data-ttu-id="2a459-276">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-276">schedule</span></span>|[<span data-ttu-id="2a459-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-278">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-279">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-280">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="2a459-281">Beispiel 3</span><span class="sxs-lookup"><span data-stu-id="2a459-281">Example 3</span></span>
<span data-ttu-id="2a459-282">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="2a459-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="2a459-283">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-283">Property</span></span>     | <span data-ttu-id="2a459-284">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-284">Type</span></span>    |<span data-ttu-id="2a459-285">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-285">Required</span></span>|  <span data-ttu-id="2a459-286">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-287">resourceId</span></span>|<span data-ttu-id="2a459-288">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-288">String</span></span>|<span data-ttu-id="2a459-289">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-289">Yes</span></span>|<span data-ttu-id="2a459-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-290">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-291">roleDefinitionId</span></span>|<span data-ttu-id="2a459-292">String</span><span class="sxs-lookup"><span data-stu-id="2a459-292">String</span></span>|<span data-ttu-id="2a459-293">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-293">Yes</span></span>|<span data-ttu-id="2a459-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-295">subjectId</span></span>|<span data-ttu-id="2a459-296">String</span><span class="sxs-lookup"><span data-stu-id="2a459-296">String</span></span>|<span data-ttu-id="2a459-297">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-297">Yes</span></span>|<span data-ttu-id="2a459-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-298">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-299">assignmentState</span></span>|<span data-ttu-id="2a459-300">String</span><span class="sxs-lookup"><span data-stu-id="2a459-300">String</span></span>|<span data-ttu-id="2a459-301">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-301">Yes</span></span>| <span data-ttu-id="2a459-302">Aktiv</span><span class="sxs-lookup"><span data-stu-id="2a459-302">Active</span></span>|
|<span data-ttu-id="2a459-303">type</span><span class="sxs-lookup"><span data-stu-id="2a459-303">type</span></span>|<span data-ttu-id="2a459-304">String</span><span class="sxs-lookup"><span data-stu-id="2a459-304">String</span></span>|<span data-ttu-id="2a459-305">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-305">Yes</span></span>| <span data-ttu-id="2a459-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="2a459-306">UserRemove</span></span>|
|<span data-ttu-id="2a459-307">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-307">reason</span></span>|<span data-ttu-id="2a459-308">String</span><span class="sxs-lookup"><span data-stu-id="2a459-308">String</span></span>| <span data-ttu-id="2a459-309">Nein</span><span class="sxs-lookup"><span data-stu-id="2a459-309">No</span></span>||
|<span data-ttu-id="2a459-310">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-310">schedule</span></span>|[<span data-ttu-id="2a459-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-312">No</span><span class="sxs-lookup"><span data-stu-id="2a459-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-313">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-314">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="2a459-315">Beispiel 4</span><span class="sxs-lookup"><span data-stu-id="2a459-315">Example 4</span></span>
<span data-ttu-id="2a459-316">In diesem Beispiel Entfernen von Administratoren die nawu@fimdev.net Benutzer aus der Rolle Leser Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="2a459-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="2a459-317">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a459-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="2a459-318">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-318">Property</span></span>     | <span data-ttu-id="2a459-319">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-319">Type</span></span>    |<span data-ttu-id="2a459-320">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-320">Required</span></span>|  <span data-ttu-id="2a459-321">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-322">resourceId</span></span>|<span data-ttu-id="2a459-323">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-323">String</span></span>|<span data-ttu-id="2a459-324">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-324">Yes</span></span>|<span data-ttu-id="2a459-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-325">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-326">roleDefinitionId</span></span>|<span data-ttu-id="2a459-327">String</span><span class="sxs-lookup"><span data-stu-id="2a459-327">String</span></span>|<span data-ttu-id="2a459-328">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-328">Yes</span></span>|<span data-ttu-id="2a459-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-330">subjectId</span></span>|<span data-ttu-id="2a459-331">String</span><span class="sxs-lookup"><span data-stu-id="2a459-331">String</span></span>|<span data-ttu-id="2a459-332">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-332">Yes</span></span>|<span data-ttu-id="2a459-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-333">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-334">assignmentState</span></span>|<span data-ttu-id="2a459-335">String</span><span class="sxs-lookup"><span data-stu-id="2a459-335">String</span></span>|<span data-ttu-id="2a459-336">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-336">Yes</span></span>| <span data-ttu-id="2a459-337">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="2a459-337">Eligible / Active</span></span>|
|<span data-ttu-id="2a459-338">type</span><span class="sxs-lookup"><span data-stu-id="2a459-338">type</span></span>|<span data-ttu-id="2a459-339">String</span><span class="sxs-lookup"><span data-stu-id="2a459-339">String</span></span>|<span data-ttu-id="2a459-340">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-340">Yes</span></span>| <span data-ttu-id="2a459-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="2a459-341">AdminRemove</span></span>|
|<span data-ttu-id="2a459-342">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-342">reason</span></span>|<span data-ttu-id="2a459-343">String</span><span class="sxs-lookup"><span data-stu-id="2a459-343">String</span></span>| <span data-ttu-id="2a459-344">Nein</span><span class="sxs-lookup"><span data-stu-id="2a459-344">No</span></span>||
|<span data-ttu-id="2a459-345">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-345">schedule</span></span>|[<span data-ttu-id="2a459-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-347">No</span><span class="sxs-lookup"><span data-stu-id="2a459-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-348">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-349">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="2a459-350">Beispiel 5</span><span class="sxs-lookup"><span data-stu-id="2a459-350">Example 5</span></span>
<span data-ttu-id="2a459-351">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="2a459-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="2a459-352">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a459-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="2a459-353">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-353">Property</span></span>     | <span data-ttu-id="2a459-354">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-354">Type</span></span>    |<span data-ttu-id="2a459-355">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-355">Required</span></span>|  <span data-ttu-id="2a459-356">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-357">resourceId</span></span>|<span data-ttu-id="2a459-358">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-358">String</span></span>|<span data-ttu-id="2a459-359">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-359">Yes</span></span>|<span data-ttu-id="2a459-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-360">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-361">roleDefinitionId</span></span>|<span data-ttu-id="2a459-362">String</span><span class="sxs-lookup"><span data-stu-id="2a459-362">String</span></span>|<span data-ttu-id="2a459-363">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-363">Yes</span></span>|<span data-ttu-id="2a459-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-365">subjectId</span></span>|<span data-ttu-id="2a459-366">String</span><span class="sxs-lookup"><span data-stu-id="2a459-366">String</span></span>|<span data-ttu-id="2a459-367">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-367">Yes</span></span>|<span data-ttu-id="2a459-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-368">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-369">assignmentState</span></span>|<span data-ttu-id="2a459-370">String</span><span class="sxs-lookup"><span data-stu-id="2a459-370">String</span></span>|<span data-ttu-id="2a459-371">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-371">Yes</span></span>| <span data-ttu-id="2a459-372">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="2a459-372">Eligible / Active</span></span>|
|<span data-ttu-id="2a459-373">type</span><span class="sxs-lookup"><span data-stu-id="2a459-373">type</span></span>|<span data-ttu-id="2a459-374">String</span><span class="sxs-lookup"><span data-stu-id="2a459-374">String</span></span>|<span data-ttu-id="2a459-375">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-375">Yes</span></span>| <span data-ttu-id="2a459-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="2a459-376">AdminUpdate</span></span>|
|<span data-ttu-id="2a459-377">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-377">reason</span></span>|<span data-ttu-id="2a459-378">String</span><span class="sxs-lookup"><span data-stu-id="2a459-378">String</span></span>| <span data-ttu-id="2a459-379">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="2a459-379">depends on roleSettings</span></span>||
|<span data-ttu-id="2a459-380">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-380">schedule</span></span>|[<span data-ttu-id="2a459-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-382">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-383">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-384">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="2a459-385">Beispiel 6</span><span class="sxs-lookup"><span data-stu-id="2a459-385">Example 6</span></span>
<span data-ttu-id="2a459-386">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="2a459-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="2a459-387">**Hinweis:** In Additon die Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a459-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="2a459-388">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a459-388">Property</span></span>     | <span data-ttu-id="2a459-389">Typ</span><span class="sxs-lookup"><span data-stu-id="2a459-389">Type</span></span>    |<span data-ttu-id="2a459-390">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a459-390">Required</span></span>|  <span data-ttu-id="2a459-391">Wert</span><span class="sxs-lookup"><span data-stu-id="2a459-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="2a459-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-392">resourceId</span></span>|<span data-ttu-id="2a459-393">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a459-393">String</span></span>|<span data-ttu-id="2a459-394">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-394">Yes</span></span>|<span data-ttu-id="2a459-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="2a459-395">\<resourceId\></span></span>|
|<span data-ttu-id="2a459-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2a459-396">roleDefinitionId</span></span>|<span data-ttu-id="2a459-397">String</span><span class="sxs-lookup"><span data-stu-id="2a459-397">String</span></span>|<span data-ttu-id="2a459-398">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-398">Yes</span></span>|<span data-ttu-id="2a459-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2a459-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="2a459-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="2a459-400">subjectId</span></span>|<span data-ttu-id="2a459-401">String</span><span class="sxs-lookup"><span data-stu-id="2a459-401">String</span></span>|<span data-ttu-id="2a459-402">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-402">Yes</span></span>|<span data-ttu-id="2a459-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2a459-403">\<subjectId\></span></span>|
|<span data-ttu-id="2a459-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2a459-404">assignmentState</span></span>|<span data-ttu-id="2a459-405">String</span><span class="sxs-lookup"><span data-stu-id="2a459-405">String</span></span>|<span data-ttu-id="2a459-406">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-406">Yes</span></span>| <span data-ttu-id="2a459-407">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="2a459-407">Eligible / Active</span></span> |
|<span data-ttu-id="2a459-408">type</span><span class="sxs-lookup"><span data-stu-id="2a459-408">type</span></span>|<span data-ttu-id="2a459-409">String</span><span class="sxs-lookup"><span data-stu-id="2a459-409">String</span></span>|<span data-ttu-id="2a459-410">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-410">Yes</span></span>| <span data-ttu-id="2a459-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="2a459-411">AdminExtend</span></span>|
|<span data-ttu-id="2a459-412">Grund</span><span class="sxs-lookup"><span data-stu-id="2a459-412">reason</span></span>|<span data-ttu-id="2a459-413">String</span><span class="sxs-lookup"><span data-stu-id="2a459-413">String</span></span>| <span data-ttu-id="2a459-414">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="2a459-414">depends on roleSettings</span></span>||
|<span data-ttu-id="2a459-415">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="2a459-415">schedule</span></span>|[<span data-ttu-id="2a459-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a459-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2a459-417">Ja</span><span class="sxs-lookup"><span data-stu-id="2a459-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="2a459-418">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a459-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="2a459-419">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a459-419">Response</span></span>
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
