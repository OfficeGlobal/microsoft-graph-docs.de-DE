---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften des GovernanceRoleSetting.
ms.openlocfilehash: 2d9417c99e63b1b4c7302c2afdda4c272b2fce82
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191116"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="e3a17-103">GovernanceRoleSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3a17-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="e3a17-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3a17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3a17-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3a17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3a17-106">Aktualisieren Sie die Eigenschaften des [GovernanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="e3a17-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3a17-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3a17-107">Permissions</span></span>
<span data-ttu-id="e3a17-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="e3a17-110">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3a17-110">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="e3a17-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3a17-111">Permission type</span></span>      | <span data-ttu-id="e3a17-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3a17-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3a17-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3a17-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e3a17-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e3a17-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e3a17-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3a17-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3a17-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3a17-116">Not supported.</span></span>    |
|<span data-ttu-id="e3a17-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3a17-117">Application</span></span> | <span data-ttu-id="e3a17-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e3a17-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3a17-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3a17-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3a17-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3a17-120">Request headers</span></span>
| <span data-ttu-id="e3a17-121">Name</span><span class="sxs-lookup"><span data-stu-id="e3a17-121">Name</span></span>       | <span data-ttu-id="e3a17-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3a17-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e3a17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a17-123">Authorization</span></span>  | <span data-ttu-id="e3a17-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e3a17-124">Bearer {code}</span></span>|
| <span data-ttu-id="e3a17-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e3a17-125">Content-type</span></span>  | <span data-ttu-id="e3a17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3a17-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="e3a17-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3a17-127">Request body</span></span>
<span data-ttu-id="e3a17-128">Geben Sie im Textkörper Anforderung die Werte für [GovernanceRuleSettings](../resources/governancerulesetting.md) , die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e3a17-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="e3a17-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3a17-129">Property</span></span>     | <span data-ttu-id="e3a17-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e3a17-130">Type</span></span>   |<span data-ttu-id="e3a17-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3a17-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3a17-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="e3a17-132">adminEligibleSettings</span></span>|[<span data-ttu-id="e3a17-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e3a17-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e3a17-134">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e3a17-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="e3a17-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e3a17-135">adminMemberSettings</span></span>|[<span data-ttu-id="e3a17-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e3a17-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e3a17-137">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e3a17-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="e3a17-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="e3a17-138">userEligibleSettings</span></span>|[<span data-ttu-id="e3a17-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e3a17-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e3a17-140">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e3a17-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="e3a17-141">Dies wird nicht unterstützt für `pimforazurerbac` Szenario vorläufig und kann in zukünftigen Szenarien zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="e3a17-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="e3a17-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e3a17-142">userMemberSettings</span></span>|[<span data-ttu-id="e3a17-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e3a17-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="e3a17-144">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e3a17-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="e3a17-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3a17-145">Response</span></span>
<span data-ttu-id="e3a17-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3a17-p104">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="e3a17-148">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="e3a17-148">Error codes</span></span>
<span data-ttu-id="e3a17-149">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="e3a17-149">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="e3a17-150">Darüber hinaus gibt es die folgenden benutzerdefinierten Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="e3a17-150">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="e3a17-151">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="e3a17-151">Error code</span></span>     | <span data-ttu-id="e3a17-152">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="e3a17-152">Error message</span></span>         | <span data-ttu-id="e3a17-153">Details</span><span class="sxs-lookup"><span data-stu-id="e3a17-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="e3a17-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e3a17-154">400 BadRequest</span></span>| <span data-ttu-id="e3a17-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="e3a17-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="e3a17-156">Die [GovernanceRoleSetting](../resources/governancerolesetting.md) ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="e3a17-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="e3a17-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e3a17-157">400 BadRequest</span></span>| <span data-ttu-id="e3a17-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="e3a17-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="e3a17-159">Die [GovernanceRuleSettings](../resources/governancerulesetting.md) Werte im Textkörper Anforderung ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="e3a17-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="e3a17-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3a17-160">Example</span></span> 
<span data-ttu-id="e3a17-161">Dieses Beispiel aktualisiert die Rolle Einstellung für benutzerdefinierte Rolle 3 im Abonnement Wingtip Toys - "Bemerkungen".</span><span class="sxs-lookup"><span data-stu-id="e3a17-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="e3a17-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3a17-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e3a17-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3a17-163">Response</span></span>
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
