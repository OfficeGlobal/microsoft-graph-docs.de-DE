---
title: Abrufen von governanceRoleDefinition
description: Abrufen der Eigenschaften und Beziehungen zwischen einer GovernanceRoleDefinition.
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511926"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="2264a-103">Abrufen von governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2264a-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2264a-104">Abrufen der Eigenschaften und Beziehungen zwischen einer [GovernanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2264a-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2264a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2264a-105">Permissions</span></span>
<span data-ttu-id="2264a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2264a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2264a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2264a-108">Permission type</span></span>      | <span data-ttu-id="2264a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2264a-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2264a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2264a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2264a-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2264a-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2264a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2264a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2264a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2264a-113">Not supported.</span></span>    |
|<span data-ttu-id="2264a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2264a-114">Application</span></span> | <span data-ttu-id="2264a-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2264a-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="2264a-116">Neben den Berechtigungsbereich benötigt diese API den Requestor mindestens eine rollenzuweisung für die Ressource verfügen, die die [GovernanceRoleDefinition](../resources/governanceroledefinition.md) gehört.</span><span class="sxs-lookup"><span data-stu-id="2264a-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="2264a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2264a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2264a-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2264a-118">Optional query parameters</span></span>
<span data-ttu-id="2264a-119">Diese Methode führt **kein** Support den [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="2264a-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2264a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2264a-120">Request headers</span></span>
| <span data-ttu-id="2264a-121">Name</span><span class="sxs-lookup"><span data-stu-id="2264a-121">Name</span></span>      |<span data-ttu-id="2264a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2264a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2264a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2264a-123">Authorization</span></span>  | <span data-ttu-id="2264a-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2264a-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="2264a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2264a-125">Request body</span></span>
<span data-ttu-id="2264a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2264a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2264a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2264a-127">Response</span></span>
<span data-ttu-id="2264a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GovernanceRoleDefinition](../resources/governanceroledefinition.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2264a-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2264a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2264a-129">Example</span></span>
<span data-ttu-id="2264a-130">In diesem Beispiel wird gezeigt, wie Details der Rollendefinition DNS-Zone Mitwirkender im Abonnement Wingtip Toys - "Bemerkungen" abgerufen.</span><span class="sxs-lookup"><span data-stu-id="2264a-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="2264a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2264a-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="2264a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2264a-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
