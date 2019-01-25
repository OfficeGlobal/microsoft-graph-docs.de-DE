---
title: Pläne auflisten
description: Dient zum Abrufen einer Liste von **plannerplan**-Objekten.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e4df80ceb12f19af4dac5ea2fb196cf3efc7fdcc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510141"
---
# <a name="list-plans"></a><span data-ttu-id="3a06f-103">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="3a06f-103">List plans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a06f-104">Dient zum Abrufen einer Liste von **plannerplan**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="3a06f-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a06f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a06f-105">Permissions</span></span>
<span data-ttu-id="3a06f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a06f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a06f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a06f-108">Permission type</span></span>      | <span data-ttu-id="3a06f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a06f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a06f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a06f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a06f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a06f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a06f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a06f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a06f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a06f-113">Not supported.</span></span>    |
|<span data-ttu-id="3a06f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a06f-114">Application</span></span> | <span data-ttu-id="3a06f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a06f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a06f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a06f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a06f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3a06f-117">Optional query parameters</span></span>
<span data-ttu-id="3a06f-118">Für diese Methode müssen [Filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) für „owner“ angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="3a06f-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a06f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a06f-119">Request headers</span></span>
| <span data-ttu-id="3a06f-120">Name</span><span class="sxs-lookup"><span data-stu-id="3a06f-120">Name</span></span>      |<span data-ttu-id="3a06f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a06f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a06f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a06f-122">Authorization</span></span>  | <span data-ttu-id="3a06f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a06f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a06f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a06f-125">Request body</span></span>
<span data-ttu-id="3a06f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a06f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a06f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a06f-127">Response</span></span>

<span data-ttu-id="3a06f-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerPlan](../resources/plannerplan.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a06f-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="3a06f-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3a06f-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3a06f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a06f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a06f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a06f-133">Request</span></span>
<span data-ttu-id="3a06f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a06f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans
```
##### <a name="response"></a><span data-ttu-id="3a06f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a06f-135">Response</span></span>
<span data-ttu-id="3a06f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a06f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planner-list-plans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
