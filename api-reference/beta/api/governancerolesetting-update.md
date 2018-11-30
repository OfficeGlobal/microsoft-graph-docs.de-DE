---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften des GovernanceRoleSetting.
ms.openlocfilehash: ca5752d51e5d59578594a12c80ae1cac316b48bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058385"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="87523-103">GovernanceRoleSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87523-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="87523-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87523-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87523-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87523-106">Aktualisieren Sie die Eigenschaften des [GovernanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="87523-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87523-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87523-107">Permissions</span></span>
<span data-ttu-id="87523-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87523-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87523-110">Permission type</span></span>      | <span data-ttu-id="87523-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87523-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87523-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87523-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87523-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="87523-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="87523-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87523-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87523-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87523-115">Not supported.</span></span>    |
|<span data-ttu-id="87523-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87523-116">Application</span></span> | <span data-ttu-id="87523-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="87523-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="87523-118">Diese API erfordert neben der Berechtigungsbereich den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="87523-118">Besides the permission scope, this API requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="87523-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87523-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="87523-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87523-120">Optional request headers</span></span>
| <span data-ttu-id="87523-121">Name</span><span class="sxs-lookup"><span data-stu-id="87523-121">Name</span></span>       | <span data-ttu-id="87523-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87523-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="87523-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87523-123">Authorization</span></span>  | <span data-ttu-id="87523-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="87523-124">Bearer {code}</span></span>|
| <span data-ttu-id="87523-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="87523-125">Content-type</span></span>  | <span data-ttu-id="87523-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87523-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="87523-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87523-127">Request body</span></span>
<span data-ttu-id="87523-128">Geben Sie im Textkörper Anforderung die Werte für [GovernanceRuleSettings](../resources/governancerulesetting.md) , die aktualisiert werden muss.</span><span class="sxs-lookup"><span data-stu-id="87523-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that needs to be updated.</span></span> 

| <span data-ttu-id="87523-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87523-129">Property</span></span>     | <span data-ttu-id="87523-130">Typ</span><span class="sxs-lookup"><span data-stu-id="87523-130">Type</span></span>   |<span data-ttu-id="87523-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87523-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87523-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="87523-132">adminEligibleSettings</span></span>|[<span data-ttu-id="87523-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="87523-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="87523-134">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="87523-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="87523-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="87523-135">adminMemberSettings</span></span>|[<span data-ttu-id="87523-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="87523-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="87523-137">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="87523-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="87523-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="87523-138">userEligibleSettings</span></span>|[<span data-ttu-id="87523-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="87523-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="87523-140">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="87523-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="87523-141">Dies wird nicht unterstützt für `pimforazurerbac` Szenario vorläufig und kann in zukünftigen Szenarien zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="87523-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="87523-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="87523-142">userMemberSettings</span></span>|[<span data-ttu-id="87523-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="87523-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="87523-144">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="87523-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="87523-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="87523-145">Response</span></span>
<span data-ttu-id="87523-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87523-p104">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="87523-148">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="87523-148">Error codes</span></span>
<span data-ttu-id="87523-149">Diese API folgt dem Standard-HTTP-Codes.</span><span class="sxs-lookup"><span data-stu-id="87523-149">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="87523-150">Außerdem werden die benutzerdefinierten Fehlercodes unten angezeigt.</span><span class="sxs-lookup"><span data-stu-id="87523-150">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="87523-151">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="87523-151">Error code</span></span>     | <span data-ttu-id="87523-152">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="87523-152">Error message</span></span>         | <span data-ttu-id="87523-153">Details</span><span class="sxs-lookup"><span data-stu-id="87523-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="87523-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="87523-154">400 BadRequest</span></span>| <span data-ttu-id="87523-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="87523-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="87523-156">Die [GovernanceRoleSetting](../resources/governancerolesetting.md) ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="87523-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="87523-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="87523-157">400 BadRequest</span></span>| <span data-ttu-id="87523-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="87523-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="87523-159">Die [GovernanceRuleSettings](../resources/governancerulesetting.md) Werte im Textkörper Anforderung ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="87523-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="87523-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87523-160">Example</span></span> 
<span data-ttu-id="87523-161">Dieses Beispiel aktualisiert die Rolle Einstellung für benutzerdefinierte Rolle 3 im Abonnement Wingtip Toys - "Bemerkungen".</span><span class="sxs-lookup"><span data-stu-id="87523-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="87523-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87523-162">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a><span data-ttu-id="87523-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="87523-163">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
