---
title: Exportieren von governanceRoleAssignmentRequests
description: Abrufen einer Auflistung von GovernanceRoleAssignmentRequests im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522427"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="07df7-103">Exportieren von governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="07df7-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07df7-104">Abrufen einer Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.</span><span class="sxs-lookup"><span data-stu-id="07df7-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="07df7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07df7-105">Permissions</span></span>
<span data-ttu-id="07df7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07df7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07df7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07df7-108">Permission type</span></span>      | <span data-ttu-id="07df7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07df7-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07df7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07df7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07df7-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="07df7-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="07df7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07df7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07df7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07df7-113">Not supported.</span></span>    |
|<span data-ttu-id="07df7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07df7-114">Application</span></span> | <span data-ttu-id="07df7-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="07df7-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="07df7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07df7-116">HTTP request</span></span>
<span data-ttu-id="07df7-117"><!-- { "blockType": "ignored" } -->Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) für eine Ressource</span><span class="sxs-lookup"><span data-stu-id="07df7-117"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="07df7-118">**Hinweis:** Neben den Berechtigungsbereich erfordert dieser Anforderung den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="07df7-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="07df7-119">Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) davon.</span><span class="sxs-lookup"><span data-stu-id="07df7-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07df7-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="07df7-120">Optional query parameters</span></span>
<span data-ttu-id="07df7-121">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="07df7-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07df7-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07df7-122">Request headers</span></span>
| <span data-ttu-id="07df7-123">Name</span><span class="sxs-lookup"><span data-stu-id="07df7-123">Name</span></span>      |<span data-ttu-id="07df7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07df7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07df7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07df7-125">Authorization</span></span>  | <span data-ttu-id="07df7-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="07df7-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="07df7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07df7-127">Request body</span></span>
<span data-ttu-id="07df7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="07df7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07df7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="07df7-129">Response</span></span>
<span data-ttu-id="07df7-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Inhalte vom Typ `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="07df7-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="07df7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07df7-131">Example</span></span>
<span data-ttu-id="07df7-132">In diesem Beispiel werden alle rollenzuweisungen als CSV-Datei in das Abonnement Wingtip Toys - "Bemerkungen" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="07df7-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="07df7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07df7-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="07df7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="07df7-134">Response</span></span>
<span data-ttu-id="07df7-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07df7-135">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-export.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
