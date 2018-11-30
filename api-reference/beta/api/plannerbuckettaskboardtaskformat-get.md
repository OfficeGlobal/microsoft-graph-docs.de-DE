---
title: plannerBucketTaskBoardTaskFormat abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.
ms.openlocfilehash: 5a2f0ad97b031ef6e1c45b75b17c816329dfe0ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060936"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="6634b-103">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="6634b-103">Get plannerBucketTaskBoardTaskFormat</span></span>

> <span data-ttu-id="6634b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6634b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6634b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6634b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6634b-106">Dient zum Abrufen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6634b-106">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6634b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6634b-107">Permissions</span></span>
<span data-ttu-id="6634b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6634b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6634b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6634b-110">Permission type</span></span>      | <span data-ttu-id="6634b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6634b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6634b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6634b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6634b-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6634b-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6634b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6634b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6634b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6634b-115">Not supported.</span></span>    |
|<span data-ttu-id="6634b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6634b-116">Application</span></span> | <span data-ttu-id="6634b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6634b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6634b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6634b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="6634b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6634b-119">Request headers</span></span>
| <span data-ttu-id="6634b-120">Name</span><span class="sxs-lookup"><span data-stu-id="6634b-120">Name</span></span>      |<span data-ttu-id="6634b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6634b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6634b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6634b-122">Authorization</span></span>  | <span data-ttu-id="6634b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6634b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6634b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6634b-125">Request body</span></span>
<span data-ttu-id="6634b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6634b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6634b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6634b-127">Response</span></span>

<span data-ttu-id="6634b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6634b-128">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="6634b-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6634b-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6634b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6634b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6634b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6634b-133">Request</span></span>
<span data-ttu-id="6634b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6634b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="6634b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6634b-135">Response</span></span>
<span data-ttu-id="6634b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6634b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->