---
title: GovernanceRoleSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften von governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: f9c851f95df340693626ff82c960243eb2f85b54
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789620"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="79924-103">GovernanceRoleSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="79924-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79924-104">Aktualisieren Sie die Eigenschaften von [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="79924-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79924-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79924-105">Permissions</span></span>
<span data-ttu-id="79924-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="79924-108">**Hinweis:** Diese API erfordert außerdem, dass die anfordernden Person über `Active` mindestens eine Administratorrollen`owner` Zuweisung `user access administrator`(oder) für die Ressource verfügt.</span><span class="sxs-lookup"><span data-stu-id="79924-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="79924-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79924-109">Permission type</span></span>      | <span data-ttu-id="79924-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79924-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79924-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79924-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79924-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="79924-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="79924-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79924-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79924-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79924-114">Not supported.</span></span>    |
|<span data-ttu-id="79924-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79924-115">Application</span></span> | <span data-ttu-id="79924-116">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="79924-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="79924-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79924-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79924-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79924-118">Request headers</span></span>
| <span data-ttu-id="79924-119">Name</span><span class="sxs-lookup"><span data-stu-id="79924-119">Name</span></span>       | <span data-ttu-id="79924-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79924-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79924-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79924-121">Authorization</span></span>  | <span data-ttu-id="79924-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79924-122">Bearer {code}</span></span>|
| <span data-ttu-id="79924-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="79924-123">Content-type</span></span>  | <span data-ttu-id="79924-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79924-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="79924-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79924-125">Request body</span></span>
<span data-ttu-id="79924-126">Geben Sie im Anforderungstext die Werte für [governanceRuleSettings](../resources/governancerulesetting.md) an, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="79924-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="79924-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79924-127">Property</span></span>     | <span data-ttu-id="79924-128">Typ</span><span class="sxs-lookup"><span data-stu-id="79924-128">Type</span></span>   |<span data-ttu-id="79924-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79924-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79924-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="79924-130">adminEligibleSettings</span></span>|<span data-ttu-id="79924-131">[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="79924-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="79924-132">Die Regeleinstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine berechtigte Rollenzuweisung hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="79924-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="79924-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="79924-133">adminMemberSettings</span></span>|<span data-ttu-id="79924-134">[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="79924-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="79924-135">Die Regeleinstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte Mitglieds Rollenzuweisung hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="79924-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="79924-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="79924-136">userEligibleSettings</span></span>|<span data-ttu-id="79924-137">[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="79924-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="79924-138">Die Regeleinstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine berechtigte Rollenzuweisung hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="79924-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="79924-139">Dies wird für `pimforazurerbac` das Szenario für jetzt nicht unterstützt und ist möglicherweise in den zukünftigen Szenarien verfügbar.</span><span class="sxs-lookup"><span data-stu-id="79924-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="79924-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="79924-140">userMemberSettings</span></span>|<span data-ttu-id="79924-141">[governanceRuleSetting](../resources/governancerulesetting.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="79924-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="79924-142">Die Regeleinstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine Rollenzuweisung zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="79924-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="79924-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="79924-143">Response</span></span>
<span data-ttu-id="79924-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79924-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="79924-146">Fehlercodes</span><span class="sxs-lookup"><span data-stu-id="79924-146">Error codes</span></span>
<span data-ttu-id="79924-147">Diese API gibt die standardmäßigen HTTP-Fehlercodes zurück.</span><span class="sxs-lookup"><span data-stu-id="79924-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="79924-148">Darüber hinaus werden die folgenden benutzerdefinierten Fehlercodes zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79924-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="79924-149">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="79924-149">Error code</span></span>     | <span data-ttu-id="79924-150">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="79924-150">Error message</span></span>         | <span data-ttu-id="79924-151">Details</span><span class="sxs-lookup"><span data-stu-id="79924-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="79924-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="79924-152">400 BadRequest</span></span>| <span data-ttu-id="79924-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="79924-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="79924-154">Die [governanceRoleSetting](../resources/governancerolesetting.md) ist nicht im System vorhanden.</span><span class="sxs-lookup"><span data-stu-id="79924-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="79924-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="79924-155">400 BadRequest</span></span>| <span data-ttu-id="79924-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="79924-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="79924-157">Die im Anforderungstext angegebenen [governanceRuleSettings](../resources/governancerulesetting.md) -Werte sind ungültig.</span><span class="sxs-lookup"><span data-stu-id="79924-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="79924-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79924-158">Example</span></span> 
<span data-ttu-id="79924-159">In diesem Beispiel wird die Rollen Einstellung für die benutzerdefinierte Rolle 3 im Abonnement "Flügelspitze Toys-Prod" aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="79924-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="79924-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79924-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="79924-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="79924-161">Response</span></span>
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
