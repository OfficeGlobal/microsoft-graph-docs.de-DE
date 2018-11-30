---
title: plannerPlanDetails abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerplandetails**-Objekts.
ms.openlocfilehash: 11873befbf5d29fcdace546a0281449e31697c8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062384"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="42f8c-103">plannerPlanDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="42f8c-103">Get plannerPlanDetails</span></span>

> <span data-ttu-id="42f8c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="42f8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42f8c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42f8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42f8c-106">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerplandetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42f8c-106">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="42f8c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42f8c-107">Permissions</span></span>
<span data-ttu-id="42f8c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f8c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42f8c-110">Permission type</span></span>      | <span data-ttu-id="42f8c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42f8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42f8c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42f8c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42f8c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f8c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42f8c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42f8c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f8c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42f8c-115">Not supported.</span></span>    |
|<span data-ttu-id="42f8c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42f8c-116">Application</span></span> | <span data-ttu-id="42f8c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42f8c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42f8c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42f8c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="42f8c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42f8c-119">Request headers</span></span>
| <span data-ttu-id="42f8c-120">Name</span><span class="sxs-lookup"><span data-stu-id="42f8c-120">Name</span></span>      |<span data-ttu-id="42f8c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42f8c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42f8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f8c-122">Authorization</span></span>  | <span data-ttu-id="42f8c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42f8c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f8c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42f8c-125">Request body</span></span>
<span data-ttu-id="42f8c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="42f8c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42f8c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="42f8c-127">Response</span></span>

<span data-ttu-id="42f8c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerPlanDetails](../resources/plannerplandetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42f8c-128">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="42f8c-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="42f8c-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="42f8c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42f8c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42f8c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42f8c-133">Request</span></span>
<span data-ttu-id="42f8c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42f8c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
##### <a name="response"></a><span data-ttu-id="42f8c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="42f8c-135">Response</span></span>
<span data-ttu-id="42f8c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42f8c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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