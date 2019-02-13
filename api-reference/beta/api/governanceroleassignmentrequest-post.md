---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967221"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c098c-104">Erstellen von governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c098c-105">Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c098c-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c098c-106">Die folgende Tabelle enthält die Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="c098c-106">The following table lists the operations.</span></span>

| <span data-ttu-id="c098c-107">Vorgang</span><span class="sxs-lookup"><span data-stu-id="c098c-107">Operation</span></span>                                   | <span data-ttu-id="c098c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="c098c-109">Zuweisen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-109">Assign a role assignment</span></span>                    | <span data-ttu-id="c098c-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c098c-110">AdminAdd</span></span>    |
| <span data-ttu-id="c098c-111">Aktivieren einer qualifizierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="c098c-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c098c-112">UserAdd</span></span>     |
| <span data-ttu-id="c098c-113">Deaktivieren einer aktivierten rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="c098c-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c098c-114">UserRemove</span></span>  |
| <span data-ttu-id="c098c-115">Entfernen einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-115">Remove a role assignment</span></span>                    | <span data-ttu-id="c098c-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c098c-116">AdminRemove</span></span> |
| <span data-ttu-id="c098c-117">Aktualisieren einer rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-117">Update a role assignment</span></span>                    | <span data-ttu-id="c098c-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c098c-118">AdminUpdate</span></span> |
| <span data-ttu-id="c098c-119">So erweitern Sie meine rollenzuweisung anfordern</span><span class="sxs-lookup"><span data-stu-id="c098c-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="c098c-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="c098c-120">UserExtend</span></span>  |
| <span data-ttu-id="c098c-121">Erweitern Sie eine rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-121">Extend a role assignment</span></span>                    | <span data-ttu-id="c098c-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c098c-122">AdminExtend</span></span> |
| <span data-ttu-id="c098c-123">Anforderung an meine abgelaufene rollenzuweisung erneuern</span><span class="sxs-lookup"><span data-stu-id="c098c-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="c098c-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="c098c-124">UserRenew</span></span>   |
| <span data-ttu-id="c098c-125">Erneuern einer abgelaufenen rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="c098c-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="c098c-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="c098c-127">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c098c-127">Permissions</span></span>

<span data-ttu-id="c098c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c098c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c098c-130">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c098c-130">Permission type</span></span>                        | <span data-ttu-id="c098c-131">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c098c-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="c098c-132">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c098c-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="c098c-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c098c-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c098c-134">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c098c-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c098c-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c098c-135">Not supported.</span></span>                            |
| <span data-ttu-id="c098c-136">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c098c-136">Application</span></span>                            | <span data-ttu-id="c098c-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c098c-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="c098c-138">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c098c-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c098c-139">Request headers</span></span>

| <span data-ttu-id="c098c-140">Name</span><span class="sxs-lookup"><span data-stu-id="c098c-140">Name</span></span>          | <span data-ttu-id="c098c-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c098c-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="c098c-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="c098c-142">Authorization</span></span> | <span data-ttu-id="c098c-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c098c-143">Bearer {code}</span></span>    |
| <span data-ttu-id="c098c-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="c098c-144">Content-type</span></span>  | <span data-ttu-id="c098c-145">application/json</span><span class="sxs-lookup"><span data-stu-id="c098c-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c098c-146">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c098c-146">Request body</span></span>

<span data-ttu-id="c098c-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c098c-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="c098c-148">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-148">Property</span></span>         | <span data-ttu-id="c098c-149">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-149">Type</span></span>                                                     | <span data-ttu-id="c098c-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c098c-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="c098c-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-151">resourceId</span></span>       | <span data-ttu-id="c098c-152">String</span><span class="sxs-lookup"><span data-stu-id="c098c-152">String</span></span>                                                   | <span data-ttu-id="c098c-153">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c098c-153">The ID of the resource.</span></span> <span data-ttu-id="c098c-154">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-154">Required.</span></span> |
| <span data-ttu-id="c098c-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-155">roleDefinitionId</span></span> | <span data-ttu-id="c098c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-156">String</span></span>                                                   | <span data-ttu-id="c098c-157">Die ID der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="c098c-157">The ID of the role definition.</span></span> <span data-ttu-id="c098c-158">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-158">Required.</span></span> |
| <span data-ttu-id="c098c-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-159">subjectId</span></span>        | <span data-ttu-id="c098c-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-160">String</span></span>                                                   | <span data-ttu-id="c098c-161">Die ID des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="c098c-161">The ID of the subject.</span></span> <span data-ttu-id="c098c-162">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-162">Required.</span></span> |
| <span data-ttu-id="c098c-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-163">assignmentState</span></span>  | <span data-ttu-id="c098c-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-164">String</span></span>                                                   | <span data-ttu-id="c098c-165">Der Status der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="c098c-165">The state of assignment.</span></span> <span data-ttu-id="c098c-166">Der Wert kann sein `Eligible` und `Active`.</span><span class="sxs-lookup"><span data-stu-id="c098c-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="c098c-167">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-167">Required.</span></span> |
| <span data-ttu-id="c098c-168">type</span><span class="sxs-lookup"><span data-stu-id="c098c-168">type</span></span>             | <span data-ttu-id="c098c-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-169">String</span></span>                                                   | <span data-ttu-id="c098c-170">Der Anforderungstyp.</span><span class="sxs-lookup"><span data-stu-id="c098c-170">The request type.</span></span> <span data-ttu-id="c098c-171">Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="c098c-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="c098c-172">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-172">Required.</span></span> |
| <span data-ttu-id="c098c-173">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-173">reason</span></span>           | <span data-ttu-id="c098c-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-174">String</span></span>                                                   | <span data-ttu-id="c098c-175">Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c098c-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="c098c-176">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-176">schedule</span></span>         | [<span data-ttu-id="c098c-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-178">Den Zeitplan der Rolle Zuordnung Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c098c-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="c098c-179">Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c098c-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="c098c-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-180">Response</span></span>

<span data-ttu-id="c098c-181">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c098c-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c098c-182">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="c098c-182">Error codes</span></span>

<span data-ttu-id="c098c-183">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="c098c-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c098c-184">Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.</span><span class="sxs-lookup"><span data-stu-id="c098c-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="c098c-185">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="c098c-185">Error code</span></span>     | <span data-ttu-id="c098c-186">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="c098c-186">Error message</span></span>                               | <span data-ttu-id="c098c-187">Details</span><span class="sxs-lookup"><span data-stu-id="c098c-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="c098c-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-188">400 BadRequest</span></span> | <span data-ttu-id="c098c-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="c098c-189">RoleNotFound</span></span>                                | <span data-ttu-id="c098c-190">Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="c098c-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c098c-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-191">400 BadRequest</span></span> | <span data-ttu-id="c098c-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="c098c-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="c098c-193">Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="c098c-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="c098c-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-194">400 BadRequest</span></span> | <span data-ttu-id="c098c-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="c098c-195">SubjectNotFound</span></span>                             | <span data-ttu-id="c098c-196">Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="c098c-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c098c-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-197">400 BadRequest</span></span> | <span data-ttu-id="c098c-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="c098c-199">Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System.</span><span class="sxs-lookup"><span data-stu-id="c098c-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="c098c-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-200">400 BadRequest</span></span> | <span data-ttu-id="c098c-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="c098c-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="c098c-202">Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c098c-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="c098c-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-203">400 BadRequest</span></span> | <span data-ttu-id="c098c-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="c098c-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="c098c-205">Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="c098c-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="c098c-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c098c-206">400 BadRequest</span></span> | <span data-ttu-id="c098c-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="c098c-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c098c-208">Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="c098c-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="c098c-209">Beispiele</span><span class="sxs-lookup"><span data-stu-id="c098c-209">Examples</span></span>

<span data-ttu-id="c098c-210">Die folgenden Beispiele zeigen, wie diese API verwendet.</span><span class="sxs-lookup"><span data-stu-id="c098c-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="c098c-211">In Beispiel 1: Administrator weist Benutzer zu einer Rolle</span><span class="sxs-lookup"><span data-stu-id="c098c-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="c098c-212">In diesem Beispiel weist ein Administrator Benutzer nawu@fimdev.net Rolle Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="c098c-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="c098c-213">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="c098c-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c098c-214">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-214">Property</span></span>         | <span data-ttu-id="c098c-215">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-215">Type</span></span>                                                     | <span data-ttu-id="c098c-216">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-216">Required</span></span>                 | <span data-ttu-id="c098c-217">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c098c-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-218">resourceId</span></span>       | <span data-ttu-id="c098c-219">String</span><span class="sxs-lookup"><span data-stu-id="c098c-219">String</span></span>                                                   | <span data-ttu-id="c098c-220">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-220">Yes</span></span>                      | <span data-ttu-id="c098c-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-221">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-222">roleDefinitionId</span></span> | <span data-ttu-id="c098c-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-223">String</span></span>                                                   | <span data-ttu-id="c098c-224">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-224">Yes</span></span>                      | <span data-ttu-id="c098c-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-226">subjectId</span></span>        | <span data-ttu-id="c098c-227">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-227">String</span></span>                                                   | <span data-ttu-id="c098c-228">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-228">Yes</span></span>                      | <span data-ttu-id="c098c-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-229">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-230">assignmentState</span></span>  | <span data-ttu-id="c098c-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-231">String</span></span>                                                   | <span data-ttu-id="c098c-232">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-232">Yes</span></span>                      | <span data-ttu-id="c098c-233">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="c098c-233">Eligible / Active</span></span> |
| <span data-ttu-id="c098c-234">type</span><span class="sxs-lookup"><span data-stu-id="c098c-234">type</span></span>             | <span data-ttu-id="c098c-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-235">String</span></span>                                                   | <span data-ttu-id="c098c-236">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-236">Yes</span></span>                      | <span data-ttu-id="c098c-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c098c-237">AdminAdd</span></span> |
| <span data-ttu-id="c098c-238">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-238">reason</span></span>           | <span data-ttu-id="c098c-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-239">String</span></span>                                                   | <span data-ttu-id="c098c-240">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="c098c-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="c098c-241">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-241">schedule</span></span>         | [<span data-ttu-id="c098c-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-243">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c098c-244">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-244">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c098c-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-245">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="c098c-246">Beispiel 2: Benutzer aktiviert zu auswählbaren Rolle</span><span class="sxs-lookup"><span data-stu-id="c098c-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="c098c-247">In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.</span><span class="sxs-lookup"><span data-stu-id="c098c-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c098c-248">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-248">Property</span></span>         | <span data-ttu-id="c098c-249">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-249">Type</span></span>                                                     | <span data-ttu-id="c098c-250">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-250">Required</span></span>                 | <span data-ttu-id="c098c-251">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c098c-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-252">resourceId</span></span>       | <span data-ttu-id="c098c-253">String</span><span class="sxs-lookup"><span data-stu-id="c098c-253">String</span></span>                                                   | <span data-ttu-id="c098c-254">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-254">Yes</span></span>                      | <span data-ttu-id="c098c-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-255">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-256">roleDefinitionId</span></span> | <span data-ttu-id="c098c-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-257">String</span></span>                                                   | <span data-ttu-id="c098c-258">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-258">Yes</span></span>                      | <span data-ttu-id="c098c-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-260">subjectId</span></span>        | <span data-ttu-id="c098c-261">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-261">String</span></span>                                                   | <span data-ttu-id="c098c-262">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-262">Yes</span></span>                      | <span data-ttu-id="c098c-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-263">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-264">assignmentState</span></span>  | <span data-ttu-id="c098c-265">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-265">String</span></span>                                                   | <span data-ttu-id="c098c-266">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-266">Yes</span></span>                      | <span data-ttu-id="c098c-267">Aktiv</span><span class="sxs-lookup"><span data-stu-id="c098c-267">Active</span></span> |
| <span data-ttu-id="c098c-268">type</span><span class="sxs-lookup"><span data-stu-id="c098c-268">type</span></span>             | <span data-ttu-id="c098c-269">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-269">String</span></span>                                                   | <span data-ttu-id="c098c-270">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-270">Yes</span></span>                      | <span data-ttu-id="c098c-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c098c-271">UserAdd</span></span> |
| <span data-ttu-id="c098c-272">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-272">reason</span></span>           | <span data-ttu-id="c098c-273">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-273">String</span></span>                                                   | <span data-ttu-id="c098c-274">hängt von der Rolle Einstellungen</span><span class="sxs-lookup"><span data-stu-id="c098c-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="c098c-275">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-275">schedule</span></span>         | [<span data-ttu-id="c098c-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-277">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c098c-278">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-278">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a><span data-ttu-id="c098c-279">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-279">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="c098c-280">Beispiel 3: Benutzer deaktiviert zugewiesene Rolle</span><span class="sxs-lookup"><span data-stu-id="c098c-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="c098c-281">In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="c098c-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c098c-282">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-282">Property</span></span>         | <span data-ttu-id="c098c-283">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-283">Type</span></span>                                                     | <span data-ttu-id="c098c-284">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-284">Required</span></span> | <span data-ttu-id="c098c-285">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c098c-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-286">resourceId</span></span>       | <span data-ttu-id="c098c-287">String</span><span class="sxs-lookup"><span data-stu-id="c098c-287">String</span></span>                                                   | <span data-ttu-id="c098c-288">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-288">Yes</span></span>      | <span data-ttu-id="c098c-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-289">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-290">roleDefinitionId</span></span> | <span data-ttu-id="c098c-291">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-291">String</span></span>                                                   | <span data-ttu-id="c098c-292">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-292">Yes</span></span>      | <span data-ttu-id="c098c-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-294">subjectId</span></span>        | <span data-ttu-id="c098c-295">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-295">String</span></span>                                                   | <span data-ttu-id="c098c-296">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-296">Yes</span></span>      | <span data-ttu-id="c098c-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-297">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-298">assignmentState</span></span>  | <span data-ttu-id="c098c-299">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-299">String</span></span>                                                   | <span data-ttu-id="c098c-300">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-300">Yes</span></span>      | <span data-ttu-id="c098c-301">Aktiv</span><span class="sxs-lookup"><span data-stu-id="c098c-301">Active</span></span> |
| <span data-ttu-id="c098c-302">type</span><span class="sxs-lookup"><span data-stu-id="c098c-302">type</span></span>             | <span data-ttu-id="c098c-303">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-303">String</span></span>                                                   | <span data-ttu-id="c098c-304">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-304">Yes</span></span>      | <span data-ttu-id="c098c-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c098c-305">UserRemove</span></span> |
| <span data-ttu-id="c098c-306">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-306">reason</span></span>           | <span data-ttu-id="c098c-307">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-307">String</span></span>                                                   | <span data-ttu-id="c098c-308">Nein</span><span class="sxs-lookup"><span data-stu-id="c098c-308">No</span></span>       |   |
| <span data-ttu-id="c098c-309">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-309">schedule</span></span>         | [<span data-ttu-id="c098c-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-311">Nein</span><span class="sxs-lookup"><span data-stu-id="c098c-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c098c-312">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-312">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a><span data-ttu-id="c098c-313">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-313">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="c098c-314">Beispiel 4: Administrator entfernt Benutzer aus einer Rolle</span><span class="sxs-lookup"><span data-stu-id="c098c-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="c098c-315">In diesem Beispiel entfernt ein Administrator die nawu@fimdev.net Benutzer aus der Abrechnung Reader-Rolle.</span><span class="sxs-lookup"><span data-stu-id="c098c-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="c098c-316">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="c098c-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c098c-317">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-317">Property</span></span>         | <span data-ttu-id="c098c-318">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-318">Type</span></span>                                                     | <span data-ttu-id="c098c-319">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-319">Required</span></span> | <span data-ttu-id="c098c-320">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c098c-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-321">resourceId</span></span>       | <span data-ttu-id="c098c-322">String</span><span class="sxs-lookup"><span data-stu-id="c098c-322">String</span></span>                                                   | <span data-ttu-id="c098c-323">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-323">Yes</span></span>      | <span data-ttu-id="c098c-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-324">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-325">roleDefinitionId</span></span> | <span data-ttu-id="c098c-326">String</span><span class="sxs-lookup"><span data-stu-id="c098c-326">String</span></span>                                                   | <span data-ttu-id="c098c-327">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-327">Yes</span></span>      | <span data-ttu-id="c098c-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-329">subjectId</span></span>        | <span data-ttu-id="c098c-330">String</span><span class="sxs-lookup"><span data-stu-id="c098c-330">String</span></span>                                                   | <span data-ttu-id="c098c-331">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-331">Yes</span></span>      | <span data-ttu-id="c098c-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-332">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-333">assignmentState</span></span>  | <span data-ttu-id="c098c-334">String</span><span class="sxs-lookup"><span data-stu-id="c098c-334">String</span></span>                                                   | <span data-ttu-id="c098c-335">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-335">Yes</span></span>      | <span data-ttu-id="c098c-336">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="c098c-336">Eligible / Active</span></span> |
| <span data-ttu-id="c098c-337">type</span><span class="sxs-lookup"><span data-stu-id="c098c-337">type</span></span>             | <span data-ttu-id="c098c-338">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-338">String</span></span>                                                   | <span data-ttu-id="c098c-339">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-339">Yes</span></span>      | <span data-ttu-id="c098c-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c098c-340">AdminRemove</span></span> |
| <span data-ttu-id="c098c-341">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-341">reason</span></span>           | <span data-ttu-id="c098c-342">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-342">String</span></span>                                                   | <span data-ttu-id="c098c-343">Nein</span><span class="sxs-lookup"><span data-stu-id="c098c-343">No</span></span>       |   |
| <span data-ttu-id="c098c-344">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-344">schedule</span></span>         | [<span data-ttu-id="c098c-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-346">Nein</span><span class="sxs-lookup"><span data-stu-id="c098c-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c098c-347">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-347">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a><span data-ttu-id="c098c-348">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-348">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="c098c-349">Beispiel 5: Administrator aktualisiert rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="c098c-350">In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.</span><span class="sxs-lookup"><span data-stu-id="c098c-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="c098c-351">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="c098c-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c098c-352">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-352">Property</span></span>         | <span data-ttu-id="c098c-353">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-353">Type</span></span>                                                     | <span data-ttu-id="c098c-354">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-354">Required</span></span>                | <span data-ttu-id="c098c-355">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c098c-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-356">resourceId</span></span>       | <span data-ttu-id="c098c-357">String</span><span class="sxs-lookup"><span data-stu-id="c098c-357">String</span></span>                                                   | <span data-ttu-id="c098c-358">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-358">Yes</span></span>                     | <span data-ttu-id="c098c-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-359">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-360">roleDefinitionId</span></span> | <span data-ttu-id="c098c-361">String</span><span class="sxs-lookup"><span data-stu-id="c098c-361">String</span></span>                                                   | <span data-ttu-id="c098c-362">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-362">Yes</span></span>                     | <span data-ttu-id="c098c-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-364">subjectId</span></span>        | <span data-ttu-id="c098c-365">String</span><span class="sxs-lookup"><span data-stu-id="c098c-365">String</span></span>                                                   | <span data-ttu-id="c098c-366">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-366">Yes</span></span>                     | <span data-ttu-id="c098c-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-367">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-368">assignmentState</span></span>  | <span data-ttu-id="c098c-369">String</span><span class="sxs-lookup"><span data-stu-id="c098c-369">String</span></span>                                                   | <span data-ttu-id="c098c-370">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-370">Yes</span></span>                     | <span data-ttu-id="c098c-371">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="c098c-371">Eligible / Active</span></span> |
| <span data-ttu-id="c098c-372">type</span><span class="sxs-lookup"><span data-stu-id="c098c-372">type</span></span>             | <span data-ttu-id="c098c-373">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-373">String</span></span>                                                   | <span data-ttu-id="c098c-374">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-374">Yes</span></span>                     | <span data-ttu-id="c098c-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c098c-375">AdminUpdate</span></span> |
| <span data-ttu-id="c098c-376">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-376">reason</span></span>           | <span data-ttu-id="c098c-377">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-377">String</span></span>                                                   | <span data-ttu-id="c098c-378">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="c098c-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c098c-379">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-379">schedule</span></span>         | [<span data-ttu-id="c098c-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-381">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c098c-382">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-382">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="c098c-383">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-383">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="c098c-384">Beispiel 6: Administrator erweitert ablaufende rollenzuweisung</span><span class="sxs-lookup"><span data-stu-id="c098c-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="c098c-385">In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.</span><span class="sxs-lookup"><span data-stu-id="c098c-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c098c-386">**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="c098c-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c098c-387">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c098c-387">Property</span></span>         | <span data-ttu-id="c098c-388">Typ</span><span class="sxs-lookup"><span data-stu-id="c098c-388">Type</span></span>                                                     | <span data-ttu-id="c098c-389">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="c098c-389">Required</span></span>                | <span data-ttu-id="c098c-390">Wert</span><span class="sxs-lookup"><span data-stu-id="c098c-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c098c-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="c098c-391">resourceId</span></span>       | <span data-ttu-id="c098c-392">String</span><span class="sxs-lookup"><span data-stu-id="c098c-392">String</span></span>                                                   | <span data-ttu-id="c098c-393">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-393">Yes</span></span>                     | <span data-ttu-id="c098c-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c098c-394">\<resourceId\></span></span> |
| <span data-ttu-id="c098c-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c098c-395">roleDefinitionId</span></span> | <span data-ttu-id="c098c-396">String</span><span class="sxs-lookup"><span data-stu-id="c098c-396">String</span></span>                                                   | <span data-ttu-id="c098c-397">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-397">Yes</span></span>                     | <span data-ttu-id="c098c-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c098c-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c098c-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="c098c-399">subjectId</span></span>        | <span data-ttu-id="c098c-400">String</span><span class="sxs-lookup"><span data-stu-id="c098c-400">String</span></span>                                                   | <span data-ttu-id="c098c-401">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-401">Yes</span></span>                     | <span data-ttu-id="c098c-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c098c-402">\<subjectId\></span></span> |
| <span data-ttu-id="c098c-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c098c-403">assignmentState</span></span>  | <span data-ttu-id="c098c-404">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-404">String</span></span>                                                   | <span data-ttu-id="c098c-405">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-405">Yes</span></span>                     | <span data-ttu-id="c098c-406">Berechtigte / Active</span><span class="sxs-lookup"><span data-stu-id="c098c-406">Eligible / Active</span></span> |
| <span data-ttu-id="c098c-407">type</span><span class="sxs-lookup"><span data-stu-id="c098c-407">type</span></span>             | <span data-ttu-id="c098c-408">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-408">String</span></span>                                                   | <span data-ttu-id="c098c-409">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-409">Yes</span></span>                     | <span data-ttu-id="c098c-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c098c-410">AdminExtend</span></span> |
| <span data-ttu-id="c098c-411">Grund</span><span class="sxs-lookup"><span data-stu-id="c098c-411">reason</span></span>           | <span data-ttu-id="c098c-412">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c098c-412">String</span></span>                                                   | <span data-ttu-id="c098c-413">hängt von roleSettings</span><span class="sxs-lookup"><span data-stu-id="c098c-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c098c-414">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="c098c-414">schedule</span></span>         | [<span data-ttu-id="c098c-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c098c-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c098c-416">Ja</span><span class="sxs-lookup"><span data-stu-id="c098c-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c098c-417">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c098c-417">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="c098c-418">Antwort</span><span class="sxs-lookup"><span data-stu-id="c098c-418">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
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
