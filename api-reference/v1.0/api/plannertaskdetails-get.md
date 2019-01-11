---
title: plannerTaskDetails abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen des **plannertaskdetails**-Objekts.
localization_priority: Normal
ms.openlocfilehash: 1ff08ac00125b1a1bb71ccaa95ef7385eb5b5ee7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804662"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="c09ee-103">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="c09ee-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="c09ee-104">Dient zum Abrufen der Eigenschaften und Beziehungen des **plannertaskdetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c09ee-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c09ee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c09ee-105">Permissions</span></span>
<span data-ttu-id="c09ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c09ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c09ee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c09ee-108">Permission type</span></span>      | <span data-ttu-id="c09ee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c09ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c09ee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c09ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c09ee-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c09ee-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c09ee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c09ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c09ee-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c09ee-113">Not supported.</span></span>    |
|<span data-ttu-id="c09ee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c09ee-114">Application</span></span> | <span data-ttu-id="c09ee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c09ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c09ee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c09ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="c09ee-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c09ee-117">Request headers</span></span>
| <span data-ttu-id="c09ee-118">Name</span><span class="sxs-lookup"><span data-stu-id="c09ee-118">Name</span></span>      |<span data-ttu-id="c09ee-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c09ee-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c09ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c09ee-120">Authorization</span></span>  | <span data-ttu-id="c09ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c09ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c09ee-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c09ee-123">Request body</span></span>
<span data-ttu-id="c09ee-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c09ee-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c09ee-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="c09ee-125">Response</span></span>

<span data-ttu-id="c09ee-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [plannerTaskDetails](../resources/plannertaskdetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c09ee-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="c09ee-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c09ee-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c09ee-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c09ee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c09ee-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c09ee-131">Request</span></span>
<span data-ttu-id="c09ee-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c09ee-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="c09ee-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c09ee-133">Response</span></span>
<span data-ttu-id="c09ee-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c09ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
