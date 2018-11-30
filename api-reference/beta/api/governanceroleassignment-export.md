---
title: Exportieren von governanceRoleAssignmentRequests
description: Abrufen einer Auflistung von GovernanceRoleAssignmentRequests im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.
ms.openlocfilehash: 8b9e64faeb8134f5b0bb964d296b1bab309021d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059980"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="b9e1a-103">Exportieren von governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="b9e1a-103">Export governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="b9e1a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e1a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9e1a-106">Abrufen einer Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e1a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9e1a-107">Permissions</span></span>
<span data-ttu-id="b9e1a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e1a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9e1a-110">Permission type</span></span>      | <span data-ttu-id="b9e1a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9e1a-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9e1a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9e1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9e1a-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b9e1a-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b9e1a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9e1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e1a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9e1a-115">Not supported.</span></span>    |
|<span data-ttu-id="b9e1a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9e1a-116">Application</span></span> | <span data-ttu-id="b9e1a-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b9e1a-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="b9e1a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e1a-118">HTTP request</span></span>
<span data-ttu-id="b9e1a-119"><!-- { "blockType": "ignored" } -->Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) für eine Ressource</span><span class="sxs-lookup"><span data-stu-id="b9e1a-119"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="b9e1a-120">**Hinweis:** Neben den Berechtigungsbereich erfordert dieser Anforderung den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="b9e1a-121">Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) davon.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-121">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9e1a-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b9e1a-122">Optional query parameters</span></span>
<span data-ttu-id="b9e1a-123">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9e1a-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9e1a-124">Request headers</span></span>
| <span data-ttu-id="b9e1a-125">Name</span><span class="sxs-lookup"><span data-stu-id="b9e1a-125">Name</span></span>      |<span data-ttu-id="b9e1a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9e1a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9e1a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e1a-127">Authorization</span></span>  | <span data-ttu-id="b9e1a-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9e1a-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e1a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9e1a-129">Request body</span></span>
<span data-ttu-id="b9e1a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e1a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e1a-131">Response</span></span>
<span data-ttu-id="b9e1a-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Inhalte vom Typ `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-132">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="b9e1a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9e1a-133">Example</span></span>
<span data-ttu-id="b9e1a-134">In diesem Beispiel werden alle rollenzuweisungen als CSV-Datei in das Abonnement Wingtip Toys - "Bemerkungen" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-134">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="b9e1a-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9e1a-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="b9e1a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9e1a-136">Response</span></span>
<span data-ttu-id="b9e1a-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9e1a-137">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
