---
title: plannerPlan abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen eines **plannerplan**-Objekts.
localization_priority: Normal
ms.openlocfilehash: 3ea9a643ab9a792106777967611223584aab2d35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839375"
---
# <a name="get-plannerplan"></a><span data-ttu-id="8a2ba-103">plannerPlan abrufen</span><span class="sxs-lookup"><span data-stu-id="8a2ba-103">Get plannerPlan</span></span>

<span data-ttu-id="8a2ba-104">Dient zum Abrufen der Eigenschaften und der Beziehungen eines **plannerplan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-104">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a2ba-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a2ba-105">Permissions</span></span>
<span data-ttu-id="8a2ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a2ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a2ba-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a2ba-108">Permission type</span></span>      | <span data-ttu-id="8a2ba-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a2ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a2ba-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a2ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a2ba-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a2ba-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a2ba-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a2ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a2ba-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a2ba-113">Not supported.</span></span>    |
|<span data-ttu-id="8a2ba-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a2ba-114">Application</span></span> | <span data-ttu-id="8a2ba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a2ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a2ba-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a2ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8a2ba-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a2ba-117">Request headers</span></span>
| <span data-ttu-id="8a2ba-118">Name</span><span class="sxs-lookup"><span data-stu-id="8a2ba-118">Name</span></span>      |<span data-ttu-id="8a2ba-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a2ba-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8a2ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a2ba-120">Authorization</span></span>  | <span data-ttu-id="8a2ba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a2ba-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a2ba-123">Request body</span></span>
<span data-ttu-id="8a2ba-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a2ba-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a2ba-125">Response</span></span>

<span data-ttu-id="8a2ba-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-126">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="8a2ba-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8a2ba-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8a2ba-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a2ba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a2ba-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a2ba-131">Request</span></span>
<span data-ttu-id="8a2ba-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
```
##### <a name="response"></a><span data-ttu-id="8a2ba-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a2ba-133">Response</span></span>
<span data-ttu-id="8a2ba-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a2ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
