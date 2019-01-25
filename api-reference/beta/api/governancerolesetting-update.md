---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften des GovernanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509329"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="252d7-103">GovernanceRoleSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="252d7-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="252d7-104">Aktualisieren Sie die Eigenschaften des [GovernanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="252d7-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="252d7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="252d7-105">Permissions</span></span>
<span data-ttu-id="252d7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="252d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="252d7-108">**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="252d7-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="252d7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="252d7-109">Permission type</span></span>      | <span data-ttu-id="252d7-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="252d7-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="252d7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="252d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="252d7-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="252d7-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="252d7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="252d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="252d7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="252d7-114">Not supported.</span></span>    |
|<span data-ttu-id="252d7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="252d7-115">Application</span></span> | <span data-ttu-id="252d7-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="252d7-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="252d7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="252d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="252d7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="252d7-118">Request headers</span></span>
| <span data-ttu-id="252d7-119">Name</span><span class="sxs-lookup"><span data-stu-id="252d7-119">Name</span></span>       | <span data-ttu-id="252d7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="252d7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="252d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="252d7-121">Authorization</span></span>  | <span data-ttu-id="252d7-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="252d7-122">Bearer {code}</span></span>|
| <span data-ttu-id="252d7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="252d7-123">Content-type</span></span>  | <span data-ttu-id="252d7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="252d7-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="252d7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="252d7-125">Request body</span></span>
<span data-ttu-id="252d7-126">Geben Sie im Textkörper Anforderung die Werte für [GovernanceRuleSettings](../resources/governancerulesetting.md) , die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="252d7-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="252d7-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="252d7-127">Property</span></span>     | <span data-ttu-id="252d7-128">Typ</span><span class="sxs-lookup"><span data-stu-id="252d7-128">Type</span></span>   |<span data-ttu-id="252d7-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="252d7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="252d7-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="252d7-130">adminEligibleSettings</span></span>|[<span data-ttu-id="252d7-131">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="252d7-131">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="252d7-132">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="252d7-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="252d7-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="252d7-133">adminMemberSettings</span></span>|[<span data-ttu-id="252d7-134">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="252d7-134">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="252d7-135">Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="252d7-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="252d7-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="252d7-136">userEligibleSettings</span></span>|[<span data-ttu-id="252d7-137">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="252d7-137">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="252d7-138">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="252d7-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="252d7-139">Dies wird nicht unterstützt für `pimforazurerbac` Szenario vorläufig und kann in zukünftigen Szenarien zur Verfügung gestellt.</span><span class="sxs-lookup"><span data-stu-id="252d7-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="252d7-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="252d7-140">userMemberSettings</span></span>|[<span data-ttu-id="252d7-141">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="252d7-141">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="252d7-142">Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="252d7-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="252d7-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="252d7-143">Response</span></span>
<span data-ttu-id="252d7-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="252d7-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="252d7-146">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="252d7-146">Error codes</span></span>
<span data-ttu-id="252d7-147">Diese API gibt die standard-HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="252d7-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="252d7-148">Darüber hinaus gibt es die folgenden benutzerdefinierten Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="252d7-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="252d7-149">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="252d7-149">Error code</span></span>     | <span data-ttu-id="252d7-150">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="252d7-150">Error message</span></span>         | <span data-ttu-id="252d7-151">Details</span><span class="sxs-lookup"><span data-stu-id="252d7-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="252d7-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="252d7-152">400 BadRequest</span></span>| <span data-ttu-id="252d7-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="252d7-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="252d7-154">Die [GovernanceRoleSetting](../resources/governancerolesetting.md) ist im System nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="252d7-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="252d7-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="252d7-155">400 BadRequest</span></span>| <span data-ttu-id="252d7-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="252d7-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="252d7-157">Die [GovernanceRuleSettings](../resources/governancerulesetting.md) Werte im Textkörper Anforderung ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="252d7-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="252d7-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="252d7-158">Example</span></span> 
<span data-ttu-id="252d7-159">Dieses Beispiel aktualisiert die Rolle Einstellung für benutzerdefinierte Rolle 3 im Abonnement Wingtip Toys - "Bemerkungen".</span><span class="sxs-lookup"><span data-stu-id="252d7-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="252d7-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="252d7-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="252d7-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="252d7-161">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
