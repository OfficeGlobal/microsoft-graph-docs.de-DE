---
title: plannerTask löschen
description: Dient zum Löschen eines **plannerTask**-Objekts.
localization_priority: Normal
ms.openlocfilehash: bf33164bf1cc97838af8dc0d8ef28395ccd03b5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820930"
---
# <a name="delete-plannertask"></a><span data-ttu-id="4d885-103">plannerTask löschen</span><span class="sxs-lookup"><span data-stu-id="4d885-103">Delete plannerTask</span></span>

<span data-ttu-id="4d885-104">Dient zum Löschen eines **plannerTask**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d885-104">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d885-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d885-105">Permissions</span></span>
<span data-ttu-id="4d885-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d885-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d885-108">Permission type</span></span>      | <span data-ttu-id="4d885-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d885-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d885-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d885-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d885-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d885-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d885-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d885-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d885-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d885-113">Not supported.</span></span>    |
|<span data-ttu-id="4d885-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d885-114">Application</span></span> | <span data-ttu-id="4d885-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d885-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d885-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d885-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4d885-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d885-117">Request headers</span></span>
| <span data-ttu-id="4d885-118">Name</span><span class="sxs-lookup"><span data-stu-id="4d885-118">Name</span></span>       | <span data-ttu-id="4d885-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d885-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d885-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d885-120">Authorization</span></span>  | <span data-ttu-id="4d885-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d885-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d885-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4d885-123">If-Match</span></span>  | <span data-ttu-id="4d885-p103">Letzter bekannter ETag-Wert für die zu löschende **plannerTask**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d885-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d885-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d885-126">Request body</span></span>
<span data-ttu-id="4d885-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d885-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d885-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d885-128">Response</span></span>

<span data-ttu-id="4d885-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d885-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="4d885-p105">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4d885-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4d885-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d885-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d885-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d885-135">Request</span></span>
<span data-ttu-id="4d885-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d885-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="4d885-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d885-137">Response</span></span>
<span data-ttu-id="4d885-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d885-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
