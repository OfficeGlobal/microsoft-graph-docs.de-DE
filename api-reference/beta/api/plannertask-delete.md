---
title: plannerTask löschen
description: Dient zum Löschen eines **plannerTask**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8d3bfe54b790d671c964112b1f12c83d6971c4d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930540"
---
# <a name="delete-plannertask"></a><span data-ttu-id="e8290-103">plannerTask löschen</span><span class="sxs-lookup"><span data-stu-id="e8290-103">Delete plannerTask</span></span>

> <span data-ttu-id="e8290-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8290-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8290-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8290-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8290-106">Dient zum Löschen eines **plannerTask**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8290-106">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8290-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8290-107">Permissions</span></span>
<span data-ttu-id="e8290-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8290-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8290-110">Permission type</span></span>      | <span data-ttu-id="e8290-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8290-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8290-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8290-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8290-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8290-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8290-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8290-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8290-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8290-115">Not supported.</span></span>    |
|<span data-ttu-id="e8290-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8290-116">Application</span></span> | <span data-ttu-id="e8290-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8290-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8290-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8290-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/<id>
```
## <a name="request-headers"></a><span data-ttu-id="e8290-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8290-119">Request headers</span></span>
| <span data-ttu-id="e8290-120">Name</span><span class="sxs-lookup"><span data-stu-id="e8290-120">Name</span></span>       | <span data-ttu-id="e8290-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8290-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8290-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8290-122">Authorization</span></span>  | <span data-ttu-id="e8290-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8290-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8290-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="e8290-125">If-Match</span></span>  | <span data-ttu-id="e8290-p104">Letzter bekannter ETag-Wert für die zu löschende **plannerTask**. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8290-p104">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8290-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8290-128">Request body</span></span>
<span data-ttu-id="e8290-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8290-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8290-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8290-130">Response</span></span>

<span data-ttu-id="e8290-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8290-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="e8290-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e8290-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e8290-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8290-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8290-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8290-137">Request</span></span>
<span data-ttu-id="e8290-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8290-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/tasks/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="e8290-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8290-139">Response</span></span>
<span data-ttu-id="e8290-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8290-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
