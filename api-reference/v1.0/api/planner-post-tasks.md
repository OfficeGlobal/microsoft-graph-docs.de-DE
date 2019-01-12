---
title: plannerTask erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen **plannerTask**-Objekts.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f628dcf4aed87f896f9a6a97682c10ecef7fec31
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990544"
---
# <a name="create-plannertask"></a><span data-ttu-id="e8d25-103">plannerTask erstellen</span><span class="sxs-lookup"><span data-stu-id="e8d25-103">Create plannerTask</span></span>

<span data-ttu-id="e8d25-104">Verwenden Sie diese API zum Erstellen eines neuen **plannerTask**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8d25-104">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8d25-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8d25-105">Permissions</span></span>
<span data-ttu-id="e8d25-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d25-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8d25-108">Permission type</span></span>      | <span data-ttu-id="e8d25-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8d25-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d25-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8d25-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8d25-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d25-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8d25-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8d25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d25-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8d25-113">Not supported.</span></span>    |
|<span data-ttu-id="e8d25-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8d25-114">Application</span></span> | <span data-ttu-id="e8d25-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8d25-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d25-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8d25-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="e8d25-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8d25-117">Request headers</span></span>
| <span data-ttu-id="e8d25-118">Name</span><span class="sxs-lookup"><span data-stu-id="e8d25-118">Name</span></span>       | <span data-ttu-id="e8d25-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8d25-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8d25-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8d25-120">Authorization</span></span>  | <span data-ttu-id="e8d25-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8d25-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8d25-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8d25-123">Request body</span></span>
<span data-ttu-id="e8d25-p103">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerTask](../resources/plannertask.md)-Objekts an. Die Eigenschaft „planId“ des **plannerTask**-Objekts muss auf die ID eines vorhandenen [plannerPlan](../resources/plannerplan.md)-Objekts festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e8d25-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="e8d25-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8d25-126">Response</span></span>

<span data-ttu-id="e8d25-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [plannerTask](../resources/plannertask.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8d25-127">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="e8d25-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e8d25-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e8d25-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8d25-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8d25-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8d25-132">Request</span></span>
<span data-ttu-id="e8d25-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8d25-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  },
}
```
<span data-ttu-id="e8d25-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerTask](../resources/plannertask.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e8d25-134">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e8d25-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8d25-135">Response</span></span>
<span data-ttu-id="e8d25-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8d25-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
