---
title: plannerBucket erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen **plannerBucket**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 03ca34760bbffd5858a2fd04b217dad49a9472d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955786"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="a24d6-103">plannerBucket erstellen</span><span class="sxs-lookup"><span data-stu-id="a24d6-103">Create plannerBucket</span></span>

> <span data-ttu-id="a24d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a24d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a24d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a24d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a24d6-106">Verwenden Sie diese API zum Erstellen eines neuen **plannerBucket**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a24d6-106">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a24d6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a24d6-107">Permissions</span></span>
<span data-ttu-id="a24d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a24d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a24d6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a24d6-110">Permission type</span></span>      | <span data-ttu-id="a24d6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a24d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a24d6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a24d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a24d6-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a24d6-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a24d6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a24d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a24d6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a24d6-115">Not supported.</span></span>    |
|<span data-ttu-id="a24d6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a24d6-116">Application</span></span> | <span data-ttu-id="a24d6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a24d6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a24d6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a24d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="a24d6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a24d6-119">Request headers</span></span>
| <span data-ttu-id="a24d6-120">Name</span><span class="sxs-lookup"><span data-stu-id="a24d6-120">Name</span></span>       | <span data-ttu-id="a24d6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a24d6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a24d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a24d6-122">Authorization</span></span>  | <span data-ttu-id="a24d6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a24d6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a24d6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a24d6-125">Request body</span></span>
<span data-ttu-id="a24d6-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerBucket](../resources/plannerbucket.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a24d6-126">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a24d6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a24d6-127">Response</span></span>

<span data-ttu-id="a24d6-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [plannerBucket](../resources/plannerbucket.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a24d6-128">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="a24d6-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a24d6-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a24d6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a24d6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a24d6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a24d6-133">Request</span></span>
<span data-ttu-id="a24d6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a24d6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="a24d6-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerBucket](../resources/plannerbucket.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a24d6-135">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a24d6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a24d6-136">Response</span></span>
<span data-ttu-id="a24d6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a24d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
