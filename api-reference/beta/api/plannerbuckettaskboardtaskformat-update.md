---
title: plannerBucketTaskBoardTaskFormat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerBucketTaskBoardTaskFormat**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ff962e09e6bb603c20c25bc835c4ac980e237a08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509042"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="9a679-103">plannerBucketTaskBoardTaskFormat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9a679-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a679-104">Dient zum Aktualisieren der Eigenschaften eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a679-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a679-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a679-105">Permissions</span></span>
<span data-ttu-id="9a679-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a679-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a679-108">Permission type</span></span>      | <span data-ttu-id="9a679-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a679-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a679-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a679-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a679-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a679-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a679-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a679-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a679-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a679-113">Not supported.</span></span>    |
|<span data-ttu-id="9a679-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a679-114">Application</span></span> | <span data-ttu-id="9a679-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a679-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a679-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a679-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a679-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a679-117">Optional request headers</span></span>
| <span data-ttu-id="9a679-118">Name</span><span class="sxs-lookup"><span data-stu-id="9a679-118">Name</span></span>       | <span data-ttu-id="9a679-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a679-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a679-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a679-120">Authorization</span></span>  | <span data-ttu-id="9a679-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a679-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a679-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="9a679-123">If-Match</span></span>  | <span data-ttu-id="9a679-p103">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerBucketTaskBoardTaskFormat**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a679-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a679-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a679-126">Request body</span></span>
<span data-ttu-id="9a679-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="9a679-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a679-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a679-130">Property</span></span>     | <span data-ttu-id="9a679-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9a679-131">Type</span></span>   |<span data-ttu-id="9a679-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a679-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a679-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="9a679-133">orderHint</span></span>|<span data-ttu-id="9a679-134">String</span><span class="sxs-lookup"><span data-stu-id="9a679-134">String</span></span>|<span data-ttu-id="9a679-p105">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](../resources/planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="9a679-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="9a679-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a679-137">Response</span></span>

<span data-ttu-id="9a679-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a679-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="9a679-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9a679-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9a679-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a679-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a679-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a679-143">Request</span></span>
<span data-ttu-id="9a679-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a679-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="9a679-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a679-145">Response</span></span>
<span data-ttu-id="9a679-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a679-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
