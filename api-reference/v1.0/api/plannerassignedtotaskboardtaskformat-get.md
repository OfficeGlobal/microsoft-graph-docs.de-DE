---
title: plannerAssignedToTaskBoardTaskFormat abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.
ms.openlocfilehash: 4c7ee2149f9250743b52f144aa0f5bc7ca85b472
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016739"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="e3c43-103">plannerAssignedToTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="e3c43-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="e3c43-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3c43-104">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3c43-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3c43-105">Permissions</span></span>
<span data-ttu-id="e3c43-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c43-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3c43-108">Permission type</span></span>      | <span data-ttu-id="e3c43-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3c43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3c43-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3c43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3c43-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c43-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3c43-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3c43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3c43-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3c43-113">Not supported.</span></span>    |
|<span data-ttu-id="e3c43-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3c43-114">Application</span></span> | <span data-ttu-id="e3c43-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3c43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3c43-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3c43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="e3c43-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3c43-117">Request headers</span></span>
| <span data-ttu-id="e3c43-118">Name</span><span class="sxs-lookup"><span data-stu-id="e3c43-118">Name</span></span>      |<span data-ttu-id="e3c43-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3c43-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3c43-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3c43-120">Authorization</span></span>  | <span data-ttu-id="e3c43-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3c43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3c43-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3c43-123">Request body</span></span>
<span data-ttu-id="e3c43-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3c43-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3c43-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3c43-125">Response</span></span>

<span data-ttu-id="e3c43-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3c43-126">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e3c43-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e3c43-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e3c43-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3c43-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3c43-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3c43-131">Request</span></span>
<span data-ttu-id="e3c43-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3c43-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="e3c43-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3c43-133">Response</span></span>
<span data-ttu-id="e3c43-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3c43-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->