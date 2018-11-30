---
title: plannerPlanDetails abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerplandetails**-Objekts.
ms.openlocfilehash: 652ba06541562f059c7e2b690b99b595e47331c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019496"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="a2800-103">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="a2800-103">Get plannerPlanDetails</span></span>

<span data-ttu-id="a2800-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerplandetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2800-104">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2800-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a2800-105">Permissions</span></span>
<span data-ttu-id="a2800-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2800-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2800-108">Permission type</span></span>      | <span data-ttu-id="a2800-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2800-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2800-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2800-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2800-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2800-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2800-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2800-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2800-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2800-113">Not supported.</span></span>    |
|<span data-ttu-id="a2800-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2800-114">Application</span></span> | <span data-ttu-id="a2800-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2800-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2800-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2800-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="a2800-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2800-117">Request headers</span></span>
| <span data-ttu-id="a2800-118">Name</span><span class="sxs-lookup"><span data-stu-id="a2800-118">Name</span></span>      |<span data-ttu-id="a2800-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2800-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2800-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2800-120">Authorization</span></span>  | <span data-ttu-id="a2800-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2800-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2800-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2800-123">Request body</span></span>
<span data-ttu-id="a2800-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a2800-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2800-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2800-125">Response</span></span>

<span data-ttu-id="a2800-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerPlanDetails](../resources/plannerplandetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2800-126">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="a2800-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a2800-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a2800-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2800-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2800-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2800-131">Request</span></span>
<span data-ttu-id="a2800-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2800-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
```
##### <a name="response"></a><span data-ttu-id="a2800-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2800-133">Response</span></span>
<span data-ttu-id="a2800-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2800-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->