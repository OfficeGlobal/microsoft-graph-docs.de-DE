---
title: 'PrivilegedApproval: MyRequests'
description: Get-Anforderungen für das jeweilige Genehmigung.
ms.openlocfilehash: 22485c1ec1127b6c8a3e1f2b40e7d052e885c357
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064609"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="6021b-103">PrivilegedApproval: MyRequests</span><span class="sxs-lookup"><span data-stu-id="6021b-103">privilegedApproval: myRequests</span></span>

> <span data-ttu-id="6021b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6021b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6021b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6021b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6021b-106">Get-Anforderungen für das jeweilige Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="6021b-106">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="6021b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6021b-107">Permissions</span></span>
<span data-ttu-id="6021b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6021b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6021b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6021b-110">Permission type</span></span>      | <span data-ttu-id="6021b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6021b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6021b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6021b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6021b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6021b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6021b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6021b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6021b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6021b-115">Not supported.</span></span>    |
|<span data-ttu-id="6021b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6021b-116">Application</span></span> | <span data-ttu-id="6021b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6021b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6021b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6021b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="6021b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6021b-119">Request headers</span></span>
| <span data-ttu-id="6021b-120">Name</span><span class="sxs-lookup"><span data-stu-id="6021b-120">Name</span></span>       | <span data-ttu-id="6021b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6021b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6021b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6021b-122">Authorization</span></span>  | <span data-ttu-id="6021b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6021b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6021b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6021b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6021b-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="6021b-126">Response</span></span>

<span data-ttu-id="6021b-127">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [PrivilegedApproval](../resources/privilegedapproval.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6021b-127">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="6021b-128">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="6021b-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6021b-129">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="6021b-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="6021b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6021b-130">Example</span></span>
<span data-ttu-id="6021b-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6021b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6021b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6021b-132">Request</span></span>
<span data-ttu-id="6021b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6021b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="6021b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6021b-134">Response</span></span>
<span data-ttu-id="6021b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6021b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
