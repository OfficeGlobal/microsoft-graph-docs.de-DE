---
title: Aufgaben auflisten
description: Dient zum Abrufen eine Liste von **plannerTask**-Objekten, die einem Benutzer zugewiesen sind.
ms.openlocfilehash: 33e852e0514806cd042092bf7692f631c367018a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065827"
---
# <a name="list-tasks"></a><span data-ttu-id="552af-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="552af-103">List tasks</span></span>

> <span data-ttu-id="552af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="552af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="552af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="552af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="552af-106">Dient zum Abrufen eine Liste von **plannerTask**-Objekten, die einem Benutzer zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="552af-106">Retrieve a list of **plannertask** objects assigned to a User.</span></span>

## <a name="permissions"></a><span data-ttu-id="552af-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="552af-107">Permissions</span></span>
<span data-ttu-id="552af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="552af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="552af-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="552af-110">Permission type</span></span>      | <span data-ttu-id="552af-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="552af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="552af-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="552af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="552af-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552af-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="552af-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="552af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="552af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="552af-115">Not supported.</span></span>    |
|<span data-ttu-id="552af-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="552af-116">Application</span></span> | <span data-ttu-id="552af-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="552af-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="552af-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="552af-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/tasks
GET /users/<id>/planner/tasks
```

## <a name="request-headers"></a><span data-ttu-id="552af-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="552af-119">Request headers</span></span>
| <span data-ttu-id="552af-120">Name</span><span class="sxs-lookup"><span data-stu-id="552af-120">Name</span></span>      |<span data-ttu-id="552af-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="552af-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="552af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="552af-122">Authorization</span></span>  | <span data-ttu-id="552af-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="552af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="552af-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="552af-125">Request body</span></span>
<span data-ttu-id="552af-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="552af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="552af-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="552af-127">Response</span></span>

<span data-ttu-id="552af-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [plannerTask](../resources/plannertask.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="552af-128">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="552af-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="552af-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="552af-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="552af-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="552af-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="552af-133">Request</span></span>
<span data-ttu-id="552af-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="552af-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="552af-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="552af-135">Response</span></span>
<span data-ttu-id="552af-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="552af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "@odata.type": "#microsoft.graph.plannerAssignment",
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