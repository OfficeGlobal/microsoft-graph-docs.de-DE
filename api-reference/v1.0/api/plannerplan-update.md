---
title: PlannerPlan aktualisieren
description: Aktualisieren Sie die Eigenschaften des **PlannerPlan** -Objekts.
localization_priority: Normal
ms.openlocfilehash: 55dcc8816489144b43c6dc41500bdee94190883d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856483"
---
# <a name="update-plannerplan"></a><span data-ttu-id="0c2f6-103">PlannerPlan aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0c2f6-103">Update plannerPlan</span></span>

<span data-ttu-id="0c2f6-104">Aktualisieren Sie die Eigenschaften des **PlannerPlan** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c2f6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0c2f6-105">Permissions</span></span>
<span data-ttu-id="0c2f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c2f6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c2f6-108">Permission type</span></span>      | <span data-ttu-id="0c2f6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c2f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c2f6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c2f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c2f6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c2f6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c2f6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c2f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c2f6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c2f6-113">Not supported.</span></span>    |
|<span data-ttu-id="0c2f6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c2f6-114">Application</span></span> | <span data-ttu-id="0c2f6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c2f6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c2f6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c2f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c2f6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c2f6-117">Request headers</span></span>

| <span data-ttu-id="0c2f6-118">Name</span><span class="sxs-lookup"><span data-stu-id="0c2f6-118">Name</span></span>       | <span data-ttu-id="0c2f6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c2f6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0c2f6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2f6-120">Authorization</span></span>  | <span data-ttu-id="0c2f6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c2f6-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="0c2f6-123">If-Match</span></span>  | <span data-ttu-id="0c2f6-p103">Letzter bekannter ETag-Wert für den zu aktualisierenden plannerPlan. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c2f6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c2f6-126">Request body</span></span>
<span data-ttu-id="0c2f6-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c2f6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c2f6-130">Property</span></span>     | <span data-ttu-id="0c2f6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0c2f6-131">Type</span></span>   |<span data-ttu-id="0c2f6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c2f6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c2f6-133">owner</span><span class="sxs-lookup"><span data-stu-id="0c2f6-133">owner</span></span>|<span data-ttu-id="0c2f6-134">String</span><span class="sxs-lookup"><span data-stu-id="0c2f6-134">String</span></span>|<span data-ttu-id="0c2f6-p105">[Gruppe](../resources/group.md) `id`, in deren Besitz der Plan ist. Dieses Feld kann erst festgelegt werden, wenn eine gültige Gruppe vorhanden ist. Nachdem dieses festgelegt wurde, kann es nur noch vom Besitzer aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="0c2f6-138">title</span><span class="sxs-lookup"><span data-stu-id="0c2f6-138">title</span></span>|<span data-ttu-id="0c2f6-139">String</span><span class="sxs-lookup"><span data-stu-id="0c2f6-139">String</span></span>|<span data-ttu-id="0c2f6-140">Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="0c2f6-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c2f6-141">Response</span></span>

<span data-ttu-id="0c2f6-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="0c2f6-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0c2f6-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c2f6-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c2f6-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c2f6-147">Request</span></span>
<span data-ttu-id="0c2f6-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="0c2f6-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c2f6-149">Response</span></span>
<span data-ttu-id="0c2f6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c2f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
