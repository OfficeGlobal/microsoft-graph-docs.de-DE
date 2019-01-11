---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
localization_priority: Normal
ms.openlocfilehash: 09adb824147dba745649efc7589ca763f815278d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823772"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="15b0d-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="15b0d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15b0d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15b0d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15b0d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15b0d-107">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="15b0d-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="15b0d-108">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="15b0d-108">The following table lists the operations.</span></span>

| <span data-ttu-id="15b0d-109">Vorgang</span><span class="sxs-lookup"><span data-stu-id="15b0d-109">Operation</span></span>       | <span data-ttu-id="15b0d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="15b0d-111">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-111">Assign a role assignment</span></span>| <span data-ttu-id="15b0d-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="15b0d-112">AdminAdd</span></span> |
| <span data-ttu-id="15b0d-113">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="15b0d-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="15b0d-114">UserAdd</span></span> | 
| <span data-ttu-id="15b0d-115">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="15b0d-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="15b0d-116">UserRemove</span></span> | 
| <span data-ttu-id="15b0d-117">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-117">Remove a role assignment</span></span>| <span data-ttu-id="15b0d-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="15b0d-118">AdminRemove</span></span> |
| <span data-ttu-id="15b0d-119">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-119">Update a role assignment</span></span>| <span data-ttu-id="15b0d-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="15b0d-120">AdminUpdate</span></span> |
| <span data-ttu-id="15b0d-121">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="15b0d-121">Request to extend my role assignment</span></span>| <span data-ttu-id="15b0d-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="15b0d-122">UserExtend</span></span> | 
| <span data-ttu-id="15b0d-123">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-123">Extend a role assignment</span></span>| <span data-ttu-id="15b0d-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="15b0d-124">AdminExtend</span></span> | 
| <span data-ttu-id="15b0d-125">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="15b0d-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="15b0d-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="15b0d-126">UserRenew</span></span> | 
| <span data-ttu-id="15b0d-127">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="15b0d-127">Renew an expired role assignment</span></span>| <span data-ttu-id="15b0d-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="15b0d-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="15b0d-129">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15b0d-129">Permissions</span></span>
<span data-ttu-id="15b0d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15b0d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15b0d-132">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15b0d-132">Permission type</span></span>      | <span data-ttu-id="15b0d-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15b0d-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15b0d-134">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15b0d-134">Delegated (work or school account)</span></span> | <span data-ttu-id="15b0d-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15b0d-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="15b0d-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15b0d-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15b0d-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15b0d-137">Not supported.</span></span>    |
|<span data-ttu-id="15b0d-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15b0d-138">Application</span></span> | <span data-ttu-id="15b0d-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15b0d-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="15b0d-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="15b0d-141">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15b0d-141">Request headers</span></span>
| <span data-ttu-id="15b0d-142">Name</span><span class="sxs-lookup"><span data-stu-id="15b0d-142">Name</span></span>       | <span data-ttu-id="15b0d-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15b0d-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15b0d-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="15b0d-144">Authorization</span></span>  | <span data-ttu-id="15b0d-145">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="15b0d-145">Bearer {code}</span></span>|
| <span data-ttu-id="15b0d-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="15b0d-146">Content-type</span></span>  | <span data-ttu-id="15b0d-147">application/json</span><span class="sxs-lookup"><span data-stu-id="15b0d-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15b0d-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15b0d-148">Request body</span></span>
<span data-ttu-id="15b0d-149">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="15b0d-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="15b0d-150">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-150">Property</span></span>     | <span data-ttu-id="15b0d-151">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-151">Type</span></span>    |<span data-ttu-id="15b0d-152">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-152">Required</span></span>|  <span data-ttu-id="15b0d-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15b0d-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-154">resourceId</span></span>|<span data-ttu-id="15b0d-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-155">String</span></span>|<span data-ttu-id="15b0d-156">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-156">Yes</span></span>|<span data-ttu-id="15b0d-157">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15b0d-157">The ID of the resource.</span></span>|
|<span data-ttu-id="15b0d-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-158">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-159">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-159">String</span></span>|<span data-ttu-id="15b0d-160">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-160">Yes</span></span>|<span data-ttu-id="15b0d-161">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="15b0d-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="15b0d-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-162">subjectId</span></span>|<span data-ttu-id="15b0d-163">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-163">String</span></span>|<span data-ttu-id="15b0d-164">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-164">Yes</span></span>|<span data-ttu-id="15b0d-165">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="15b0d-165">The ID of the subject.</span></span>|
|<span data-ttu-id="15b0d-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-166">assignmentState</span></span>|<span data-ttu-id="15b0d-167">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-167">String</span></span>|<span data-ttu-id="15b0d-168">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-168">Yes</span></span>|<span data-ttu-id="15b0d-169">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="15b0d-169">The state of assignment.</span></span> <span data-ttu-id="15b0d-170">Der Wert kann sein ``Eligible`` und ``Active``.</span><span class="sxs-lookup"><span data-stu-id="15b0d-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="15b0d-171">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-171">type</span></span>|<span data-ttu-id="15b0d-172">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-172">String</span></span>|<span data-ttu-id="15b0d-173">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-173">Yes</span></span>|<span data-ttu-id="15b0d-174">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="15b0d-174">The request type.</span></span> <span data-ttu-id="15b0d-175">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="15b0d-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="15b0d-176">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-176">reason</span></span>|<span data-ttu-id="15b0d-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-177">String</span></span>| |<span data-ttu-id="15b0d-178">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="15b0d-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="15b0d-179">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-179">schedule</span></span>|[<span data-ttu-id="15b0d-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="15b0d-181">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15b0d-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="15b0d-182">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15b0d-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="15b0d-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-183">Response</span></span>
<span data-ttu-id="15b0d-184">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="15b0d-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="15b0d-185">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="15b0d-185">Error codes</span></span>
<span data-ttu-id="15b0d-186">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="15b0d-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="15b0d-187">Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.</span><span class="sxs-lookup"><span data-stu-id="15b0d-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="15b0d-188">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="15b0d-188">Error code</span></span>     | <span data-ttu-id="15b0d-189">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="15b0d-189">Error message</span></span>              | <span data-ttu-id="15b0d-190">Details</span><span class="sxs-lookup"><span data-stu-id="15b0d-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="15b0d-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-191">400 BadRequest</span></span> | <span data-ttu-id="15b0d-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="15b0d-192">RoleNotFound</span></span>    | <span data-ttu-id="15b0d-193">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="15b0d-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="15b0d-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-194">400 BadRequest</span></span> | <span data-ttu-id="15b0d-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="15b0d-195">ResourceIsLocked</span></span>    | <span data-ttu-id="15b0d-196">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="15b0d-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="15b0d-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-197">400 BadRequest</span></span> | <span data-ttu-id="15b0d-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="15b0d-198">SubjectNotFound</span></span>    | <span data-ttu-id="15b0d-199">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="15b0d-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="15b0d-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-200">400 BadRequest</span></span> | <span data-ttu-id="15b0d-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="15b0d-202">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="15b0d-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="15b0d-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-203">400 BadRequest</span></span> | <span data-ttu-id="15b0d-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="15b0d-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="15b0d-205">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="15b0d-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="15b0d-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-206">400 BadRequest</span></span> | <span data-ttu-id="15b0d-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="15b0d-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="15b0d-208">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="15b0d-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="15b0d-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="15b0d-209">400 BadRequest</span></span> | <span data-ttu-id="15b0d-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="15b0d-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="15b0d-211">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="15b0d-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="15b0d-212">Beispiele</span><span class="sxs-lookup"><span data-stu-id="15b0d-212">Examples</span></span>
<span data-ttu-id="15b0d-213">Die folgenden Beispiele zeigen, wie diese API verwendet.</span><span class="sxs-lookup"><span data-stu-id="15b0d-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="15b0d-214">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="15b0d-214">Example 1</span></span>
<span data-ttu-id="15b0d-215">In diesem Beispiel weisen Sie Administratoren Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="15b0d-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="15b0d-216">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="15b0d-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="15b0d-217">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-217">Property</span></span>     | <span data-ttu-id="15b0d-218">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-218">Type</span></span>    |<span data-ttu-id="15b0d-219">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-219">Required</span></span>|  <span data-ttu-id="15b0d-220">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-221">resourceId</span></span>|<span data-ttu-id="15b0d-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-222">String</span></span>|<span data-ttu-id="15b0d-223">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-223">Yes</span></span>|<span data-ttu-id="15b0d-224">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-224">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-225">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-226">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-226">String</span></span>|<span data-ttu-id="15b0d-227">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-227">Yes</span></span>|<span data-ttu-id="15b0d-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-229">subjectId</span></span>|<span data-ttu-id="15b0d-230">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-230">String</span></span>|<span data-ttu-id="15b0d-231">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-231">Yes</span></span>|<span data-ttu-id="15b0d-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-232">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-233">assignmentState</span></span>|<span data-ttu-id="15b0d-234">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-234">String</span></span>|<span data-ttu-id="15b0d-235">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-235">Yes</span></span>| <span data-ttu-id="15b0d-236">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="15b0d-236">Eligible / Active</span></span>|
|<span data-ttu-id="15b0d-237">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-237">type</span></span>|<span data-ttu-id="15b0d-238">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-238">String</span></span>|<span data-ttu-id="15b0d-239">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-239">Yes</span></span>| <span data-ttu-id="15b0d-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="15b0d-240">AdminAdd</span></span>|
|<span data-ttu-id="15b0d-241">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-241">reason</span></span>|<span data-ttu-id="15b0d-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-242">String</span></span>| <span data-ttu-id="15b0d-243">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="15b0d-243">depends on role Settings</span></span>||
|<span data-ttu-id="15b0d-244">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-244">schedule</span></span>|[<span data-ttu-id="15b0d-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-246">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="15b0d-249">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="15b0d-249">Example 2</span></span>
<span data-ttu-id="15b0d-250">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="15b0d-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="15b0d-251">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-251">Property</span></span>     | <span data-ttu-id="15b0d-252">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-252">Type</span></span>    |<span data-ttu-id="15b0d-253">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-253">Required</span></span>|  <span data-ttu-id="15b0d-254">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-255">resourceId</span></span>|<span data-ttu-id="15b0d-256">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-256">String</span></span>|<span data-ttu-id="15b0d-257">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-257">Yes</span></span>|<span data-ttu-id="15b0d-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-258">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-259">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-260">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-260">String</span></span>|<span data-ttu-id="15b0d-261">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-261">Yes</span></span>|<span data-ttu-id="15b0d-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-263">subjectId</span></span>|<span data-ttu-id="15b0d-264">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-264">String</span></span>|<span data-ttu-id="15b0d-265">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-265">Yes</span></span>|<span data-ttu-id="15b0d-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-266">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-267">assignmentState</span></span>|<span data-ttu-id="15b0d-268">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-268">String</span></span>|<span data-ttu-id="15b0d-269">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-269">Yes</span></span>| <span data-ttu-id="15b0d-270">Aktiv</span><span class="sxs-lookup"><span data-stu-id="15b0d-270">Active</span></span>|
|<span data-ttu-id="15b0d-271">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-271">type</span></span>|<span data-ttu-id="15b0d-272">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-272">String</span></span>|<span data-ttu-id="15b0d-273">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-273">Yes</span></span>| <span data-ttu-id="15b0d-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="15b0d-274">UserAdd</span></span>|
|<span data-ttu-id="15b0d-275">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-275">reason</span></span>|<span data-ttu-id="15b0d-276">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-276">String</span></span>| <span data-ttu-id="15b0d-277">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="15b0d-277">depends on role Settings</span></span>||
|<span data-ttu-id="15b0d-278">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-278">schedule</span></span>|[<span data-ttu-id="15b0d-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-280">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-281">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-282">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="15b0d-283">Beispiel 3</span><span class="sxs-lookup"><span data-stu-id="15b0d-283">Example 3</span></span>
<span data-ttu-id="15b0d-284">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="15b0d-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="15b0d-285">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-285">Property</span></span>     | <span data-ttu-id="15b0d-286">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-286">Type</span></span>    |<span data-ttu-id="15b0d-287">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-287">Required</span></span>|  <span data-ttu-id="15b0d-288">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-289">resourceId</span></span>|<span data-ttu-id="15b0d-290">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-290">String</span></span>|<span data-ttu-id="15b0d-291">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-291">Yes</span></span>|<span data-ttu-id="15b0d-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-292">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-293">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-294">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-294">String</span></span>|<span data-ttu-id="15b0d-295">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-295">Yes</span></span>|<span data-ttu-id="15b0d-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-297">subjectId</span></span>|<span data-ttu-id="15b0d-298">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-298">String</span></span>|<span data-ttu-id="15b0d-299">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-299">Yes</span></span>|<span data-ttu-id="15b0d-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-300">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-301">assignmentState</span></span>|<span data-ttu-id="15b0d-302">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-302">String</span></span>|<span data-ttu-id="15b0d-303">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-303">Yes</span></span>| <span data-ttu-id="15b0d-304">Aktiv</span><span class="sxs-lookup"><span data-stu-id="15b0d-304">Active</span></span>|
|<span data-ttu-id="15b0d-305">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-305">type</span></span>|<span data-ttu-id="15b0d-306">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-306">String</span></span>|<span data-ttu-id="15b0d-307">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-307">Yes</span></span>| <span data-ttu-id="15b0d-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="15b0d-308">UserRemove</span></span>|
|<span data-ttu-id="15b0d-309">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-309">reason</span></span>|<span data-ttu-id="15b0d-310">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-310">String</span></span>| <span data-ttu-id="15b0d-311">Nein</span><span class="sxs-lookup"><span data-stu-id="15b0d-311">No</span></span>||
|<span data-ttu-id="15b0d-312">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-312">schedule</span></span>|[<span data-ttu-id="15b0d-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-314">Nein</span><span class="sxs-lookup"><span data-stu-id="15b0d-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-315">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-316">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-316">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="15b0d-317">Beispiel 4</span><span class="sxs-lookup"><span data-stu-id="15b0d-317">Example 4</span></span>
<span data-ttu-id="15b0d-318">In diesem Beispiel Entfernen von Administratoren die nawu@fimdev.net Benutzer aus der Rolle Leser Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="15b0d-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="15b0d-319">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="15b0d-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="15b0d-320">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-320">Property</span></span>     | <span data-ttu-id="15b0d-321">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-321">Type</span></span>    |<span data-ttu-id="15b0d-322">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-322">Required</span></span>|  <span data-ttu-id="15b0d-323">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-324">resourceId</span></span>|<span data-ttu-id="15b0d-325">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-325">String</span></span>|<span data-ttu-id="15b0d-326">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-326">Yes</span></span>|<span data-ttu-id="15b0d-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-327">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-328">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-329">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-329">String</span></span>|<span data-ttu-id="15b0d-330">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-330">Yes</span></span>|<span data-ttu-id="15b0d-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-332">subjectId</span></span>|<span data-ttu-id="15b0d-333">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-333">String</span></span>|<span data-ttu-id="15b0d-334">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-334">Yes</span></span>|<span data-ttu-id="15b0d-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-335">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-336">assignmentState</span></span>|<span data-ttu-id="15b0d-337">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-337">String</span></span>|<span data-ttu-id="15b0d-338">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-338">Yes</span></span>| <span data-ttu-id="15b0d-339">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="15b0d-339">Eligible / Active</span></span>|
|<span data-ttu-id="15b0d-340">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-340">type</span></span>|<span data-ttu-id="15b0d-341">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-341">String</span></span>|<span data-ttu-id="15b0d-342">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-342">Yes</span></span>| <span data-ttu-id="15b0d-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="15b0d-343">AdminRemove</span></span>|
|<span data-ttu-id="15b0d-344">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-344">reason</span></span>|<span data-ttu-id="15b0d-345">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-345">String</span></span>| <span data-ttu-id="15b0d-346">Nein</span><span class="sxs-lookup"><span data-stu-id="15b0d-346">No</span></span>||
|<span data-ttu-id="15b0d-347">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-347">schedule</span></span>|[<span data-ttu-id="15b0d-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-349">Nein</span><span class="sxs-lookup"><span data-stu-id="15b0d-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-350">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-351">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-351">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="15b0d-352">Beispiel 5</span><span class="sxs-lookup"><span data-stu-id="15b0d-352">Example 5</span></span>
<span data-ttu-id="15b0d-353">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="15b0d-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="15b0d-354">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="15b0d-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="15b0d-355">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-355">Property</span></span>     | <span data-ttu-id="15b0d-356">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-356">Type</span></span>    |<span data-ttu-id="15b0d-357">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-357">Required</span></span>|  <span data-ttu-id="15b0d-358">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-359">resourceId</span></span>|<span data-ttu-id="15b0d-360">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-360">String</span></span>|<span data-ttu-id="15b0d-361">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-361">Yes</span></span>|<span data-ttu-id="15b0d-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-362">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-363">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-364">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-364">String</span></span>|<span data-ttu-id="15b0d-365">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-365">Yes</span></span>|<span data-ttu-id="15b0d-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-367">subjectId</span></span>|<span data-ttu-id="15b0d-368">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-368">String</span></span>|<span data-ttu-id="15b0d-369">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-369">Yes</span></span>|<span data-ttu-id="15b0d-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-370">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-371">assignmentState</span></span>|<span data-ttu-id="15b0d-372">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-372">String</span></span>|<span data-ttu-id="15b0d-373">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-373">Yes</span></span>| <span data-ttu-id="15b0d-374">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="15b0d-374">Eligible / Active</span></span>|
|<span data-ttu-id="15b0d-375">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-375">type</span></span>|<span data-ttu-id="15b0d-376">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-376">String</span></span>|<span data-ttu-id="15b0d-377">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-377">Yes</span></span>| <span data-ttu-id="15b0d-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="15b0d-378">AdminUpdate</span></span>|
|<span data-ttu-id="15b0d-379">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-379">reason</span></span>|<span data-ttu-id="15b0d-380">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-380">String</span></span>| <span data-ttu-id="15b0d-381">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="15b0d-381">depends on roleSettings</span></span>||
|<span data-ttu-id="15b0d-382">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-382">schedule</span></span>|[<span data-ttu-id="15b0d-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-384">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-385">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-386">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="15b0d-387">Beispiel 6</span><span class="sxs-lookup"><span data-stu-id="15b0d-387">Example 6</span></span>
<span data-ttu-id="15b0d-388">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="15b0d-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="15b0d-389">**Hinweis:** In Additon die Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="15b0d-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="15b0d-390">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15b0d-390">Property</span></span>     | <span data-ttu-id="15b0d-391">Typ</span><span class="sxs-lookup"><span data-stu-id="15b0d-391">Type</span></span>    |<span data-ttu-id="15b0d-392">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b0d-392">Required</span></span>|  <span data-ttu-id="15b0d-393">Wert</span><span class="sxs-lookup"><span data-stu-id="15b0d-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="15b0d-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="15b0d-394">resourceId</span></span>|<span data-ttu-id="15b0d-395">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-395">String</span></span>|<span data-ttu-id="15b0d-396">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-396">Yes</span></span>|<span data-ttu-id="15b0d-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-397">\<resourceId\></span></span>|
|<span data-ttu-id="15b0d-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="15b0d-398">roleDefinitionId</span></span>|<span data-ttu-id="15b0d-399">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-399">String</span></span>|<span data-ttu-id="15b0d-400">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-400">Yes</span></span>|<span data-ttu-id="15b0d-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="15b0d-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="15b0d-402">subjectId</span></span>|<span data-ttu-id="15b0d-403">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-403">String</span></span>|<span data-ttu-id="15b0d-404">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-404">Yes</span></span>|<span data-ttu-id="15b0d-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="15b0d-405">\<subjectId\></span></span>|
|<span data-ttu-id="15b0d-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="15b0d-406">assignmentState</span></span>|<span data-ttu-id="15b0d-407">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-407">String</span></span>|<span data-ttu-id="15b0d-408">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-408">Yes</span></span>| <span data-ttu-id="15b0d-409">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="15b0d-409">Eligible / Active</span></span> |
|<span data-ttu-id="15b0d-410">type</span><span class="sxs-lookup"><span data-stu-id="15b0d-410">type</span></span>|<span data-ttu-id="15b0d-411">String</span><span class="sxs-lookup"><span data-stu-id="15b0d-411">String</span></span>|<span data-ttu-id="15b0d-412">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-412">Yes</span></span>| <span data-ttu-id="15b0d-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="15b0d-413">AdminExtend</span></span>|
|<span data-ttu-id="15b0d-414">Grund</span><span class="sxs-lookup"><span data-stu-id="15b0d-414">reason</span></span>|<span data-ttu-id="15b0d-415">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b0d-415">String</span></span>| <span data-ttu-id="15b0d-416">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="15b0d-416">depends on roleSettings</span></span>||
|<span data-ttu-id="15b0d-417">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="15b0d-417">schedule</span></span>|[<span data-ttu-id="15b0d-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="15b0d-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="15b0d-419">Ja</span><span class="sxs-lookup"><span data-stu-id="15b0d-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="15b0d-420">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b0d-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="15b0d-421">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b0d-421">Response</span></span>
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
