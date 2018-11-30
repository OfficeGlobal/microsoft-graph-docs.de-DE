---
title: PlannerPlan aktualisieren
description: Aktualisieren Sie die Eigenschaften des **PlannerPlan** -Objekts.
ms.openlocfilehash: 477246b442971693c2748d9f2cde10ac46b8ef0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066055"
---
# <a name="update-plannerplan"></a><span data-ttu-id="12fc1-103">PlannerPlan aktualisieren</span><span class="sxs-lookup"><span data-stu-id="12fc1-103">Update plannerPlan</span></span>

> <span data-ttu-id="12fc1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12fc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12fc1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12fc1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12fc1-106">Aktualisieren Sie die Eigenschaften des **PlannerPlan** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="12fc1-106">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12fc1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12fc1-107">Permissions</span></span>
<span data-ttu-id="12fc1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fc1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12fc1-110">Permission type</span></span>      | <span data-ttu-id="12fc1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12fc1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12fc1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12fc1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12fc1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fc1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="12fc1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12fc1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fc1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fc1-115">Not supported.</span></span>    |
|<span data-ttu-id="12fc1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12fc1-116">Application</span></span> | <span data-ttu-id="12fc1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fc1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12fc1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fc1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```

## <a name="request-headers"></a><span data-ttu-id="12fc1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12fc1-119">Request headers</span></span>

| <span data-ttu-id="12fc1-120">Name</span><span class="sxs-lookup"><span data-stu-id="12fc1-120">Name</span></span>       | <span data-ttu-id="12fc1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fc1-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="12fc1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fc1-122">Authorization</span></span>  | <span data-ttu-id="12fc1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12fc1-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="12fc1-125">If-Match</span></span>  | <span data-ttu-id="12fc1-p104">Letzter bekannter ETag-Wert für den zu aktualisierenden plannerPlan. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p104">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fc1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12fc1-128">Request body</span></span>
<span data-ttu-id="12fc1-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="12fc1-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12fc1-132">Property</span></span>     | <span data-ttu-id="12fc1-133">Typ</span><span class="sxs-lookup"><span data-stu-id="12fc1-133">Type</span></span>   |<span data-ttu-id="12fc1-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fc1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12fc1-135">owner</span><span class="sxs-lookup"><span data-stu-id="12fc1-135">owner</span></span>|<span data-ttu-id="12fc1-136">String</span><span class="sxs-lookup"><span data-stu-id="12fc1-136">String</span></span>|<span data-ttu-id="12fc1-p106">[Gruppe](../resources/group.md) `id`, in deren Besitz der Plan ist. Dieses Feld kann erst festgelegt werden, wenn eine gültige Gruppe vorhanden ist. Nachdem dieses festgelegt wurde, kann es nur noch vom Besitzer aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p106">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="12fc1-140">title</span><span class="sxs-lookup"><span data-stu-id="12fc1-140">title</span></span>|<span data-ttu-id="12fc1-141">String</span><span class="sxs-lookup"><span data-stu-id="12fc1-141">String</span></span>|<span data-ttu-id="12fc1-142">Der Titel des Plans.</span><span class="sxs-lookup"><span data-stu-id="12fc1-142">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="12fc1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fc1-143">Response</span></span>

<span data-ttu-id="12fc1-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fc1-144">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="12fc1-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="12fc1-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="12fc1-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12fc1-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12fc1-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fc1-149">Request</span></span>
<span data-ttu-id="12fc1-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12fc1-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/<id>
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="12fc1-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fc1-151">Response</span></span>
<span data-ttu-id="12fc1-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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