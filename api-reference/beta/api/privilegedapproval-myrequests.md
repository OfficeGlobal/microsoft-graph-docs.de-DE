---
title: 'PrivilegedApproval: MyRequests'
description: Get-Anforderungen für das jeweilige Genehmigung.
localization_priority: Normal
ms.openlocfilehash: 9fcbdab424c98633a8f543875b9b7c2275894df0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512892"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="a3c7b-103">PrivilegedApproval: MyRequests</span><span class="sxs-lookup"><span data-stu-id="a3c7b-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3c7b-104">Get-Anforderungen für das jeweilige Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3c7b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a3c7b-105">Permissions</span></span>
<span data-ttu-id="a3c7b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3c7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a3c7b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3c7b-108">Permission type</span></span>      | <span data-ttu-id="a3c7b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3c7b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3c7b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3c7b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3c7b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3c7b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3c7b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3c7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3c7b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3c7b-113">Not supported.</span></span>    |
|<span data-ttu-id="a3c7b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3c7b-114">Application</span></span> | <span data-ttu-id="a3c7b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3c7b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3c7b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3c7b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="a3c7b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3c7b-117">Request headers</span></span>
| <span data-ttu-id="a3c7b-118">Name</span><span class="sxs-lookup"><span data-stu-id="a3c7b-118">Name</span></span>       | <span data-ttu-id="a3c7b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3c7b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a3c7b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3c7b-120">Authorization</span></span>  | <span data-ttu-id="a3c7b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3c7b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3c7b-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a3c7b-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3c7b-124">Response</span></span>

<span data-ttu-id="a3c7b-125">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedApproval](../resources/privilegedapproval.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="a3c7b-126">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a3c7b-127">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="a3c7b-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3c7b-128">Example</span></span>
<span data-ttu-id="a3c7b-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a3c7b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3c7b-130">Request</span></span>
<span data-ttu-id="a3c7b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="a3c7b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3c7b-132">Response</span></span>
<span data-ttu-id="a3c7b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3c7b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
