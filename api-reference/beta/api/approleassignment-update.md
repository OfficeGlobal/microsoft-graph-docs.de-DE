---
title: Approleassignment aktualisieren
description: Aktualisieren Sie die Eigenschaften des Approleassignment-Objekts.
localization_priority: Normal
ms.openlocfilehash: 54c256e3b94a5bb2d62c2ffe31ecf777d472b93c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527920"
---
# <a name="update-approleassignment"></a><span data-ttu-id="67e03-103">Approleassignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="67e03-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67e03-104">Aktualisieren Sie die Eigenschaften des Approleassignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="67e03-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67e03-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67e03-105">Permissions</span></span>
<span data-ttu-id="67e03-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67e03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67e03-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67e03-108">Permission type</span></span>      | <span data-ttu-id="67e03-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67e03-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67e03-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67e03-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67e03-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67e03-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="67e03-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67e03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67e03-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67e03-113">Not supported.</span></span>    |
|<span data-ttu-id="67e03-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67e03-114">Application</span></span> | <span data-ttu-id="67e03-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67e03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67e03-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67e03-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="67e03-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67e03-117">Request headers</span></span>
| <span data-ttu-id="67e03-118">Name</span><span class="sxs-lookup"><span data-stu-id="67e03-118">Name</span></span>       | <span data-ttu-id="67e03-119">Typ</span><span class="sxs-lookup"><span data-stu-id="67e03-119">Type</span></span> | <span data-ttu-id="67e03-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67e03-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67e03-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e03-121">Authorization</span></span>  | <span data-ttu-id="67e03-122">string</span><span class="sxs-lookup"><span data-stu-id="67e03-122">string</span></span>  | <span data-ttu-id="67e03-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67e03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67e03-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67e03-125">Request body</span></span>
<span data-ttu-id="67e03-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="67e03-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67e03-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67e03-129">Property</span></span>     | <span data-ttu-id="67e03-130">Typ</span><span class="sxs-lookup"><span data-stu-id="67e03-130">Type</span></span>   |<span data-ttu-id="67e03-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67e03-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67e03-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="67e03-132">creationTimestamp</span></span>|<span data-ttu-id="67e03-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e03-133">DateTimeOffset</span></span>|<span data-ttu-id="67e03-134">Die Uhrzeit der Erstellung der erteilen.</span><span class="sxs-lookup"><span data-stu-id="67e03-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="67e03-135">id</span><span class="sxs-lookup"><span data-stu-id="67e03-135">id</span></span>|<span data-ttu-id="67e03-136">Guid</span><span class="sxs-lookup"><span data-stu-id="67e03-136">Guid</span></span>|<span data-ttu-id="67e03-137">Die Rolle-Id, die den Prinzipal zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="67e03-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="67e03-138">Diese Rolle muss mit der Ziel-Ressource Anwendung **ResourceId** in seiner **AppRoles** -Eigenschaft deklariert werden.</span><span class="sxs-lookup"><span data-stu-id="67e03-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="67e03-139">In denen die Ressource keine Berechtigungen nicht deklarieren, muss eine Standard-Id (0 (null) GUID) angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="67e03-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="67e03-140">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="67e03-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="67e03-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="67e03-141">principalDisplayName</span></span>|<span data-ttu-id="67e03-142">String</span><span class="sxs-lookup"><span data-stu-id="67e03-142">String</span></span>|<span data-ttu-id="67e03-143">Der Anzeigename des Prinzipals, die der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="67e03-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="67e03-144">principalId</span><span class="sxs-lookup"><span data-stu-id="67e03-144">principalId</span></span>|<span data-ttu-id="67e03-145">Guid</span><span class="sxs-lookup"><span data-stu-id="67e03-145">Guid</span></span>|<span data-ttu-id="67e03-146">Der eindeutige Bezeichner (**ObjectId**) für den Prinzipal, den Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="67e03-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="67e03-147">**Notes**: erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67e03-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="67e03-148">principalType</span><span class="sxs-lookup"><span data-stu-id="67e03-148">principalType</span></span>|<span data-ttu-id="67e03-149">String</span><span class="sxs-lookup"><span data-stu-id="67e03-149">String</span></span>|<span data-ttu-id="67e03-150">Der Typ des Prinzipals.</span><span class="sxs-lookup"><span data-stu-id="67e03-150">The type of principal.</span></span>  <span data-ttu-id="67e03-151">Dies kann entweder "User", "Group" oder "ServicePrincipal" sein.</span><span class="sxs-lookup"><span data-stu-id="67e03-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="67e03-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="67e03-152">resourceDisplayName</span></span>|<span data-ttu-id="67e03-153">String</span><span class="sxs-lookup"><span data-stu-id="67e03-153">String</span></span>|<span data-ttu-id="67e03-154">Der Anzeigename der Ressource mit der die Zuordnung hergestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="67e03-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="67e03-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="67e03-155">resourceId</span></span>|<span data-ttu-id="67e03-156">Guid</span><span class="sxs-lookup"><span data-stu-id="67e03-156">Guid</span></span>|<span data-ttu-id="67e03-157">Der eindeutige Bezeichner (**ObjectId**) für die Zielressource (Service Principal) für die die Zuordnung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="67e03-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="67e03-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="67e03-158">Response</span></span>

<span data-ttu-id="67e03-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [AppRoleAssignment](../resources/approleassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="67e03-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67e03-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67e03-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67e03-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67e03-161">Request</span></span>
<span data-ttu-id="67e03-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67e03-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{id}
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="67e03-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="67e03-163">Response</span></span>
<span data-ttu-id="67e03-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67e03-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
