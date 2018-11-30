---
title: Liste governanceRoleDefinitions
description: Rufen Sie eine Auflistung von GovernanceRoleDefinitions für eine Ressource.
ms.openlocfilehash: ed1d4e7b51d20ed6687c52364399385054db9912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062779"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="f20db-103">Liste governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f20db-103">List governanceRoleDefinitions</span></span>
> <span data-ttu-id="f20db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f20db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f20db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f20db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f20db-106">Rufen Sie eine Auflistung von [GovernanceRoleDefinitions](../resources/governanceroledefinition.md) für eine Ressource.</span><span class="sxs-lookup"><span data-stu-id="f20db-106">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f20db-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f20db-107">Permissions</span></span>
<span data-ttu-id="f20db-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f20db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f20db-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f20db-110">Permission type</span></span>      | <span data-ttu-id="f20db-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f20db-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f20db-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f20db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f20db-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f20db-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f20db-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f20db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f20db-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f20db-115">Not supported.</span></span>    |
|<span data-ttu-id="f20db-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f20db-116">Application</span></span> | <span data-ttu-id="f20db-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f20db-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="f20db-118">Neben den Berechtigungsbereich benötigt diese API den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f20db-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="f20db-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f20db-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f20db-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f20db-120">Optional query parameters</span></span>
<span data-ttu-id="f20db-121">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="f20db-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f20db-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f20db-122">Request headers</span></span>
| <span data-ttu-id="f20db-123">Name</span><span class="sxs-lookup"><span data-stu-id="f20db-123">Name</span></span>      |<span data-ttu-id="f20db-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f20db-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f20db-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f20db-125">Authorization</span></span>  | <span data-ttu-id="f20db-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f20db-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f20db-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f20db-127">Request body</span></span>
<span data-ttu-id="f20db-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f20db-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f20db-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f20db-129">Response</span></span>
<span data-ttu-id="f20db-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [GovernanceRoleDefinition](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f20db-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f20db-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f20db-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="f20db-132">In diesem Beispiel wird gezeigt, wie alle Rollendefinitionen des Abonnements Wingtip Toys - "Bemerkungen" abgerufen.</span><span class="sxs-lookup"><span data-stu-id="f20db-132">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f20db-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f20db-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="f20db-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f20db-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
