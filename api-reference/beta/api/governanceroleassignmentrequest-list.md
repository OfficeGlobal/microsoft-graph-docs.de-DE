---
title: Liste governanceRoleAssignmentRequests
description: 'Eine Auflistung der GovernanceRoleAssignmentRequests abzurufen. '
localization_priority: Normal
ms.openlocfilehash: 5ad26ef352eae93e9c804cfb62f5d00df12e32ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515461"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="212a8-103">Liste governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="212a8-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="212a8-104">Eine Auflistung der [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)abzurufen.</span><span class="sxs-lookup"><span data-stu-id="212a8-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="212a8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="212a8-105">Permissions</span></span>
<span data-ttu-id="212a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="212a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="212a8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="212a8-108">Permission type</span></span>      | <span data-ttu-id="212a8-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="212a8-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="212a8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="212a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="212a8-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="212a8-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="212a8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="212a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="212a8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="212a8-113">Not supported.</span></span>    |
|<span data-ttu-id="212a8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="212a8-114">Application</span></span> | <span data-ttu-id="212a8-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="212a8-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="212a8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="212a8-116">HTTP request</span></span>
<span data-ttu-id="212a8-117"><!-- { "blockType": "ignored" } -->Eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) für eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="212a8-117"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="212a8-118">**Hinweis:** Neben den Berechtigungsbereich erfordert die Anforderung den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="212a8-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="212a8-119">Eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) Meine aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="212a8-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="212a8-120">Eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , die ausstehende Administrator Entscheidungen sind aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="212a8-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="212a8-121">**Hinweis:** Neben den Berechtigungsbereich erfordert dieser Anforderung den Requestor in mindestens einem `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="212a8-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="212a8-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="212a8-122">Optional query parameters</span></span>
<span data-ttu-id="212a8-123">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="212a8-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="212a8-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="212a8-124">Request headers</span></span>
| <span data-ttu-id="212a8-125">Name</span><span class="sxs-lookup"><span data-stu-id="212a8-125">Name</span></span>      |<span data-ttu-id="212a8-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="212a8-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="212a8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="212a8-127">Authorization</span></span>  | <span data-ttu-id="212a8-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="212a8-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="212a8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="212a8-129">Request body</span></span>
<span data-ttu-id="212a8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="212a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="212a8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="212a8-131">Response</span></span>
<span data-ttu-id="212a8-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="212a8-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="212a8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="212a8-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="212a8-134">Administratoren Abfragen ausstehende Role Assignment Anforderungen für Abonnement Wingtip Toys - "Bemerkungen".</span><span class="sxs-lookup"><span data-stu-id="212a8-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="212a8-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="212a8-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="212a8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="212a8-136">Response</span></span>
<span data-ttu-id="212a8-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="212a8-137">Here is an example of the response.</span></span> 

><span data-ttu-id="212a8-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="212a8-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
                "statusDetails": [
                    {
                        "key": "EligibilityRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ExpirationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "MfaRule",
                        "value": "Grant"
                    },
                    {
                        "key": "JustificationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ActivationDayRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ApprovalRule",
                        "value": "Grant"
                    }
                ]
            },
            "schedule": {
                "type": "Once",
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
