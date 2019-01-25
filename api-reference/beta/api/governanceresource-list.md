---
title: Liste governanceResources
description: Abrufen einer Auflistung von GovernanceResource, die der Requestor auf zugreifen.
localization_priority: Normal
ms.openlocfilehash: 998e18a0139f0cbe41901da935faee2f7f24e9eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525668"
---
# <a name="list-governanceresources"></a><span data-ttu-id="1a87b-103">Liste governanceResources</span><span class="sxs-lookup"><span data-stu-id="1a87b-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a87b-104">Abrufen einer Auflistung von [GovernanceResource](../resources/governanceresource.md) , die der Requestor auf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1a87b-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a87b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a87b-105">Permissions</span></span>
<span data-ttu-id="1a87b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a87b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a87b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a87b-108">Permission type</span></span>      | <span data-ttu-id="1a87b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a87b-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a87b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a87b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a87b-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1a87b-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="1a87b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a87b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a87b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a87b-113">Not supported.</span></span>    |
|<span data-ttu-id="1a87b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a87b-114">Application</span></span> | <span data-ttu-id="1a87b-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1a87b-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a87b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a87b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a87b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1a87b-117">Optional query parameters</span></span>
<span data-ttu-id="1a87b-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="1a87b-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a87b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a87b-119">Request headers</span></span>
| <span data-ttu-id="1a87b-120">Name</span><span class="sxs-lookup"><span data-stu-id="1a87b-120">Name</span></span>      |<span data-ttu-id="1a87b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a87b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a87b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a87b-122">Authorization</span></span>  | <span data-ttu-id="1a87b-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1a87b-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a87b-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a87b-124">Request body</span></span>
<span data-ttu-id="1a87b-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a87b-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1a87b-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a87b-126">Response</span></span>
<span data-ttu-id="1a87b-127">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [GovernanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="1a87b-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="1a87b-128">Beispiele</span><span class="sxs-lookup"><span data-stu-id="1a87b-128">Examples</span></span>

<span data-ttu-id="1a87b-129">In diesem Beispiel werden alle Ressourcen, die ich derzeit zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="1a87b-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="1a87b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a87b-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="1a87b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a87b-131">Response</span></span>
<span data-ttu-id="1a87b-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a87b-132">Here is an example of the response.</span></span> 

><span data-ttu-id="1a87b-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1a87b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1289

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources",
    "value":[
        {
            "id": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/AnujRG/providers/Microsoft.Storage/storageAccounts/anujstoragefimdev",
            "type": "Microsoft.Storage/storageAccounts",
            "displayName": "anujstoragefimdev",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
