---
title: Liste governanceRoleDefinitions
description: Rufen Sie eine Auflistung von GovernanceRoleDefinitions für eine Ressource.
localization_priority: Normal
ms.openlocfilehash: 0e03a75446723743cc43eef63c42dd0f39c86126
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525199"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="a8554-103">Liste governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a8554-103">List governanceRoleDefinitions</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8554-104">Rufen Sie eine Auflistung von [GovernanceRoleDefinitions](../resources/governanceroledefinition.md) für eine Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8554-104">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8554-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8554-105">Permissions</span></span>
<span data-ttu-id="a8554-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8554-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8554-108">Permission type</span></span>      | <span data-ttu-id="a8554-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8554-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8554-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8554-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8554-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a8554-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a8554-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8554-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8554-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8554-113">Not supported.</span></span>    |
|<span data-ttu-id="a8554-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8554-114">Application</span></span> | <span data-ttu-id="a8554-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a8554-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="a8554-116">Neben den Berechtigungsbereich benötigt diese API den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="a8554-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8554-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8554-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a8554-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8554-118">Optional query parameters</span></span>
<span data-ttu-id="a8554-119">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="a8554-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8554-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8554-120">Request headers</span></span>
| <span data-ttu-id="a8554-121">Name</span><span class="sxs-lookup"><span data-stu-id="a8554-121">Name</span></span>      |<span data-ttu-id="a8554-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8554-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8554-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8554-123">Authorization</span></span>  | <span data-ttu-id="a8554-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a8554-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8554-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8554-125">Request body</span></span>
<span data-ttu-id="a8554-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a8554-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a8554-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8554-127">Response</span></span>
<span data-ttu-id="a8554-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [GovernanceRoleDefinition](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a8554-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8554-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8554-129">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="a8554-130">In diesem Beispiel wird gezeigt, wie alle Rollendefinitionen des Abonnements Wingtip Toys - "Bemerkungen" abgerufen.</span><span class="sxs-lookup"><span data-stu-id="a8554-130">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="a8554-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8554-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="a8554-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8554-132">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
