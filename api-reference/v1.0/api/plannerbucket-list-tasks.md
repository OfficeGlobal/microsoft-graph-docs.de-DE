---
title: Aufgaben auflisten
description: Dient zum Abrufen einer Liste von **plannerTask**-Objekten, die einem plannerBucket-Objekt zugeordnet sind.
ms.openlocfilehash: 4cceadabdbcc75eeba0e3285b34127713078a48f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019982"
---
# <a name="list-tasks"></a><span data-ttu-id="d7746-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="d7746-103">List tasks</span></span>

<span data-ttu-id="d7746-104">Dient zum Abrufen einer Liste von **plannerTask**-Objekten, die einem [plannerBucket](../resources/plannerbucket.md)-Objekt zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="d7746-104">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7746-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7746-105">Permissions</span></span>
<span data-ttu-id="d7746-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7746-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7746-108">Permission type</span></span>      | <span data-ttu-id="d7746-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7746-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7746-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7746-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7746-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7746-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7746-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7746-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7746-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7746-113">Not supported.</span></span>    |
|<span data-ttu-id="d7746-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7746-114">Application</span></span> | <span data-ttu-id="d7746-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7746-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7746-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7746-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="d7746-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7746-117">Request headers</span></span>
| <span data-ttu-id="d7746-118">Name</span><span class="sxs-lookup"><span data-stu-id="d7746-118">Name</span></span>      |<span data-ttu-id="d7746-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7746-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7746-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7746-120">Authorization</span></span>  | <span data-ttu-id="d7746-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7746-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7746-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7746-123">Request body</span></span>
<span data-ttu-id="d7746-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7746-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7746-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7746-125">Response</span></span>

<span data-ttu-id="d7746-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerTask](../resources/plannertask.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7746-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="d7746-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d7746-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d7746-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7746-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7746-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7746-131">Request</span></span>
<span data-ttu-id="d7746-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7746-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{task-id}/tasks
```
##### <a name="response"></a><span data-ttu-id="d7746-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7746-133">Response</span></span>
<span data-ttu-id="d7746-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7746-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerassignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->