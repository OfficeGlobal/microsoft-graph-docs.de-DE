---
title: plannerBucket löschen
description: Dient zum Löschen eines **plannerBucket**-Objekts.
ms.openlocfilehash: 43ec9c8481482ef7ea3eadab0c5a9e2c0a3b356e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018333"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="d74c7-103">plannerBucket löschen</span><span class="sxs-lookup"><span data-stu-id="d74c7-103">Delete plannerBucket</span></span>

<span data-ttu-id="d74c7-104">Dient zum Löschen eines **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d74c7-104">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="d74c7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d74c7-105">Permissions</span></span>
<span data-ttu-id="d74c7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d74c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74c7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d74c7-108">Permission type</span></span>      | <span data-ttu-id="d74c7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d74c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d74c7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d74c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d74c7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74c7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d74c7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d74c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d74c7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d74c7-113">Not supported.</span></span>    |
|<span data-ttu-id="d74c7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d74c7-114">Application</span></span> | <span data-ttu-id="d74c7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d74c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d74c7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d74c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d74c7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d74c7-117">Request headers</span></span>
| <span data-ttu-id="d74c7-118">Name</span><span class="sxs-lookup"><span data-stu-id="d74c7-118">Name</span></span>       | <span data-ttu-id="d74c7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d74c7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d74c7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d74c7-120">Authorization</span></span>  | <span data-ttu-id="d74c7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d74c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d74c7-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="d74c7-123">If-Match</span></span>  | <span data-ttu-id="d74c7-p103">Letzter bekannter ETag-Wert für den zu löschenden **plannerBucket**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d74c7-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d74c7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d74c7-126">Request body</span></span>
<span data-ttu-id="d74c7-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d74c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d74c7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d74c7-128">Response</span></span>

<span data-ttu-id="d74c7-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d74c7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d74c7-p105">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d74c7-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d74c7-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d74c7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d74c7-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d74c7-135">Request</span></span>
<span data-ttu-id="d74c7-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d74c7-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/buckets/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="d74c7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="d74c7-137">Response</span></span>
<span data-ttu-id="d74c7-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d74c7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->