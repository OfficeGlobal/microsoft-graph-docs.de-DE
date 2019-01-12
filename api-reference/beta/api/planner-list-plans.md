---
title: Pläne auflisten
description: Dient zum Abrufen einer Liste von **plannerplan**-Objekten.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9b6a8639957196e0dc5acfed861743a74e5750c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943438"
---
# <a name="list-plans"></a><span data-ttu-id="75e9a-103">Pläne auflisten</span><span class="sxs-lookup"><span data-stu-id="75e9a-103">List plans</span></span>

> <span data-ttu-id="75e9a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="75e9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75e9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75e9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75e9a-106">Dient zum Abrufen einer Liste von **plannerplan**-Objekten.</span><span class="sxs-lookup"><span data-stu-id="75e9a-106">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="75e9a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75e9a-107">Permissions</span></span>
<span data-ttu-id="75e9a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75e9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75e9a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75e9a-110">Permission type</span></span>      | <span data-ttu-id="75e9a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75e9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75e9a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75e9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75e9a-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75e9a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75e9a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75e9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75e9a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75e9a-115">Not supported.</span></span>    |
|<span data-ttu-id="75e9a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75e9a-116">Application</span></span> | <span data-ttu-id="75e9a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75e9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75e9a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75e9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75e9a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="75e9a-119">Optional query parameters</span></span>
<span data-ttu-id="75e9a-120">Für diese Methode müssen [Filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) für „owner“ angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="75e9a-120">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75e9a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75e9a-121">Request headers</span></span>
| <span data-ttu-id="75e9a-122">Name</span><span class="sxs-lookup"><span data-stu-id="75e9a-122">Name</span></span>      |<span data-ttu-id="75e9a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75e9a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75e9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="75e9a-124">Authorization</span></span>  | <span data-ttu-id="75e9a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="75e9a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75e9a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75e9a-127">Request body</span></span>
<span data-ttu-id="75e9a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="75e9a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75e9a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="75e9a-129">Response</span></span>

<span data-ttu-id="75e9a-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerPlan](../resources/plannerplan.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75e9a-130">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="75e9a-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="75e9a-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="75e9a-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75e9a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75e9a-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75e9a-135">Request</span></span>
<span data-ttu-id="75e9a-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75e9a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans
```
##### <a name="response"></a><span data-ttu-id="75e9a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="75e9a-137">Response</span></span>
<span data-ttu-id="75e9a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75e9a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
