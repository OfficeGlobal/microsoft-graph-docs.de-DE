---
title: Liste governanceResources
description: Abrufen einer Auflistung von GovernanceResource, die der Requestor auf zugreifen.
ms.openlocfilehash: a8f0fc03dbd880c82bca7c9d8f6e84a2940511d9
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191088"
---
# <a name="list-governanceresources"></a><span data-ttu-id="7dda9-103">Liste governanceResources</span><span class="sxs-lookup"><span data-stu-id="7dda9-103">List governanceResources</span></span>

> <span data-ttu-id="7dda9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7dda9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dda9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7dda9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7dda9-106">Abrufen einer Auflistung von [GovernanceResource](../resources/governanceresource.md) , die der Requestor auf zugreifen.</span><span class="sxs-lookup"><span data-stu-id="7dda9-106">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dda9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7dda9-107">Permissions</span></span>
<span data-ttu-id="7dda9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dda9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dda9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7dda9-110">Permission type</span></span>      | <span data-ttu-id="7dda9-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7dda9-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dda9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7dda9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7dda9-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7dda9-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="7dda9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7dda9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dda9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7dda9-115">Not supported.</span></span>    |
|<span data-ttu-id="7dda9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7dda9-116">Application</span></span> | <span data-ttu-id="7dda9-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7dda9-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dda9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7dda9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7dda9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7dda9-119">Optional query parameters</span></span>
<span data-ttu-id="7dda9-120">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="7dda9-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dda9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7dda9-121">Request headers</span></span>
| <span data-ttu-id="7dda9-122">Name</span><span class="sxs-lookup"><span data-stu-id="7dda9-122">Name</span></span>      |<span data-ttu-id="7dda9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7dda9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7dda9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dda9-124">Authorization</span></span>  | <span data-ttu-id="7dda9-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7dda9-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dda9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7dda9-126">Request body</span></span>
<span data-ttu-id="7dda9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7dda9-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7dda9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7dda9-128">Response</span></span>
<span data-ttu-id="7dda9-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [GovernanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="7dda9-129">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7dda9-130">Beispiele</span><span class="sxs-lookup"><span data-stu-id="7dda9-130">Examples</span></span>

<span data-ttu-id="7dda9-131">In diesem Beispiel werden alle Ressourcen, die ich derzeit zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="7dda9-131">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="7dda9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7dda9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="7dda9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7dda9-133">Response</span></span>
<span data-ttu-id="7dda9-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7dda9-134">Here is an example of the response.</span></span> 

><span data-ttu-id="7dda9-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7dda9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
