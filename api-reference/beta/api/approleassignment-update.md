---
title: Approleassignment aktualisieren
description: Aktualisieren Sie die Eigenschaften des Approleassignment-Objekts.
ms.openlocfilehash: 3c861afde396d9cab2f745c15c7de1d9a81c5dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058710"
---
# <a name="update-approleassignment"></a><span data-ttu-id="df71a-103">Approleassignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="df71a-103">Update approleassignment</span></span>

> <span data-ttu-id="df71a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df71a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df71a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df71a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df71a-106">Aktualisieren Sie die Eigenschaften des Approleassignment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="df71a-106">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="df71a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="df71a-107">Permissions</span></span>
<span data-ttu-id="df71a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df71a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df71a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df71a-110">Permission type</span></span>      | <span data-ttu-id="df71a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df71a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df71a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df71a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df71a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df71a-113">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="df71a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df71a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df71a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df71a-115">Not supported.</span></span>    |
|<span data-ttu-id="df71a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df71a-116">Application</span></span> | <span data-ttu-id="df71a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df71a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df71a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df71a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="df71a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df71a-119">Request headers</span></span>
| <span data-ttu-id="df71a-120">Name</span><span class="sxs-lookup"><span data-stu-id="df71a-120">Name</span></span>       | <span data-ttu-id="df71a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="df71a-121">Type</span></span> | <span data-ttu-id="df71a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df71a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="df71a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df71a-123">Authorization</span></span>  | <span data-ttu-id="df71a-124">string</span><span class="sxs-lookup"><span data-stu-id="df71a-124">string</span></span>  | <span data-ttu-id="df71a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df71a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df71a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df71a-127">Request body</span></span>
<span data-ttu-id="df71a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="df71a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="df71a-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df71a-131">Property</span></span>     | <span data-ttu-id="df71a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="df71a-132">Type</span></span>   |<span data-ttu-id="df71a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df71a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df71a-134">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="df71a-134">creationTimestamp</span></span>|<span data-ttu-id="df71a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df71a-135">DateTimeOffset</span></span>|<span data-ttu-id="df71a-136">Die Uhrzeit der Erstellung der erteilen.</span><span class="sxs-lookup"><span data-stu-id="df71a-136">The time when the grant was created.</span></span>|
|<span data-ttu-id="df71a-137">id</span><span class="sxs-lookup"><span data-stu-id="df71a-137">id</span></span>|<span data-ttu-id="df71a-138">Guid</span><span class="sxs-lookup"><span data-stu-id="df71a-138">Guid</span></span>|<span data-ttu-id="df71a-139">Die Rolle-Id, die den Prinzipal zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="df71a-139">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="df71a-140">Diese Rolle muss mit der Ziel-Ressource Anwendung **ResourceId** in seiner **AppRoles** -Eigenschaft deklariert werden.</span><span class="sxs-lookup"><span data-stu-id="df71a-140">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="df71a-141">In denen die Ressource keine Berechtigungen nicht deklarieren, muss eine Standard-Id (0 (null) GUID) angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="df71a-141">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="df71a-142">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="df71a-142">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="df71a-143">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="df71a-143">principalDisplayName</span></span>|<span data-ttu-id="df71a-144">String</span><span class="sxs-lookup"><span data-stu-id="df71a-144">String</span></span>|<span data-ttu-id="df71a-145">Der Anzeigename des Prinzipals, die der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="df71a-145">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="df71a-146">principalId</span><span class="sxs-lookup"><span data-stu-id="df71a-146">principalId</span></span>|<span data-ttu-id="df71a-147">Guid</span><span class="sxs-lookup"><span data-stu-id="df71a-147">Guid</span></span>|<span data-ttu-id="df71a-148">Der eindeutige Bezeichner (**ObjectId**) für den Prinzipal, den Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="df71a-148">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="df71a-149">**Notes**: erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df71a-149">**Notes**: required.</span></span>            |
|<span data-ttu-id="df71a-150">principalType</span><span class="sxs-lookup"><span data-stu-id="df71a-150">principalType</span></span>|<span data-ttu-id="df71a-151">String</span><span class="sxs-lookup"><span data-stu-id="df71a-151">String</span></span>|<span data-ttu-id="df71a-152">Der Typ des Prinzipals.</span><span class="sxs-lookup"><span data-stu-id="df71a-152">The type of principal.</span></span>  <span data-ttu-id="df71a-153">Dies kann entweder "User", "Group" oder "ServicePrincipal" sein.</span><span class="sxs-lookup"><span data-stu-id="df71a-153">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="df71a-154">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="df71a-154">resourceDisplayName</span></span>|<span data-ttu-id="df71a-155">String</span><span class="sxs-lookup"><span data-stu-id="df71a-155">String</span></span>|<span data-ttu-id="df71a-156">Der Anzeigename der Ressource mit der die Zuordnung hergestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="df71a-156">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="df71a-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="df71a-157">resourceId</span></span>|<span data-ttu-id="df71a-158">Guid</span><span class="sxs-lookup"><span data-stu-id="df71a-158">Guid</span></span>|<span data-ttu-id="df71a-159">Der eindeutige Bezeichner (**ObjectId**) für die Zielressource (Service Principal) für die die Zuordnung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="df71a-159">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="df71a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="df71a-160">Response</span></span>

<span data-ttu-id="df71a-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [AppRoleAssignment](../resources/approleassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="df71a-161">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df71a-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df71a-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df71a-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df71a-163">Request</span></span>
<span data-ttu-id="df71a-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df71a-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="df71a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="df71a-165">Response</span></span>
<span data-ttu-id="df71a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df71a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->