---
title: plannerProgressTaskBoardTaskFormat abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4100d7d5e2f5f12f22508c87433738737aa8d054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510071"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="8914b-103">plannerProgressTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="8914b-103">Get plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8914b-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8914b-104">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8914b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8914b-105">Permissions</span></span>
<span data-ttu-id="8914b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8914b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8914b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8914b-108">Permission type</span></span>      | <span data-ttu-id="8914b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8914b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8914b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8914b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8914b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8914b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8914b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8914b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8914b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8914b-113">Not supported.</span></span>    |
|<span data-ttu-id="8914b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8914b-114">Application</span></span> | <span data-ttu-id="8914b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8914b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8914b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8914b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="8914b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8914b-117">Request headers</span></span>
| <span data-ttu-id="8914b-118">Name</span><span class="sxs-lookup"><span data-stu-id="8914b-118">Name</span></span>      |<span data-ttu-id="8914b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8914b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8914b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8914b-120">Authorization</span></span>  | <span data-ttu-id="8914b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8914b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8914b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8914b-123">Request body</span></span>
<span data-ttu-id="8914b-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8914b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8914b-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8914b-125">Response</span></span>

<span data-ttu-id="8914b-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8914b-126">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="8914b-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8914b-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8914b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8914b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8914b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8914b-131">Request</span></span>
<span data-ttu-id="8914b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8914b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="8914b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8914b-133">Response</span></span>
<span data-ttu-id="8914b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8914b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
