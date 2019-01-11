---
title: plannertaskdetails aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannertaskdetails**-Objekts.
localization_priority: Normal
ms.openlocfilehash: b87688c91a3fe33439c15c403ff248b171a3241e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840194"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="36cee-103">plannertaskdetails aktualisieren</span><span class="sxs-lookup"><span data-stu-id="36cee-103">Update plannertaskdetails</span></span>

<span data-ttu-id="36cee-104">Dient zum Aktualisieren der Eigenschaften eines **plannertaskdetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36cee-104">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36cee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="36cee-105">Permissions</span></span>
<span data-ttu-id="36cee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36cee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36cee-108">Permission type</span></span>      | <span data-ttu-id="36cee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36cee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36cee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36cee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36cee-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36cee-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36cee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36cee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36cee-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36cee-113">Not supported.</span></span>    |
|<span data-ttu-id="36cee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36cee-114">Application</span></span> | <span data-ttu-id="36cee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36cee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36cee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36cee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="36cee-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36cee-117">Optional request headers</span></span>
| <span data-ttu-id="36cee-118">Name</span><span class="sxs-lookup"><span data-stu-id="36cee-118">Name</span></span>       | <span data-ttu-id="36cee-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36cee-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36cee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="36cee-120">Authorization</span></span>  | <span data-ttu-id="36cee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36cee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36cee-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="36cee-123">If-Match</span></span>  | <span data-ttu-id="36cee-p103">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerTaskDetails**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36cee-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36cee-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36cee-126">Request body</span></span>
<span data-ttu-id="36cee-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="36cee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36cee-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36cee-130">Property</span></span>     | <span data-ttu-id="36cee-131">Typ</span><span class="sxs-lookup"><span data-stu-id="36cee-131">Type</span></span>   |<span data-ttu-id="36cee-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36cee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36cee-133">checklist</span><span class="sxs-lookup"><span data-stu-id="36cee-133">checklist</span></span>|[<span data-ttu-id="36cee-134">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="36cee-134">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="36cee-135">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="36cee-135">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="36cee-136">description</span><span class="sxs-lookup"><span data-stu-id="36cee-136">description</span></span>|<span data-ttu-id="36cee-137">String</span><span class="sxs-lookup"><span data-stu-id="36cee-137">String</span></span>|<span data-ttu-id="36cee-138">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="36cee-138">Description of the task</span></span>|
|<span data-ttu-id="36cee-139">previewType</span><span class="sxs-lookup"><span data-stu-id="36cee-139">previewType</span></span>|<span data-ttu-id="36cee-140">string</span><span class="sxs-lookup"><span data-stu-id="36cee-140">string</span></span>|<span data-ttu-id="36cee-141">Hierdurch wird den Typ der Vorschau, die für den Vorgang wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="36cee-141">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="36cee-142">Die möglichen Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="36cee-142">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="36cee-143">Bei Festlegung auf `automatic` die angezeigte Vorschau wird von der app anzeigen den Vorgang ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="36cee-143">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="36cee-144">references</span><span class="sxs-lookup"><span data-stu-id="36cee-144">references</span></span>|[<span data-ttu-id="36cee-145">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="36cee-145">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="36cee-146">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="36cee-146">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="36cee-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="36cee-147">Response</span></span>

<span data-ttu-id="36cee-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerTaskDetails](../resources/plannertaskdetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36cee-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="36cee-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="36cee-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="36cee-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36cee-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36cee-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36cee-153">Request</span></span>
<span data-ttu-id="36cee-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36cee-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
Content-type: application/json
Content-length: 857
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "previewType": "noPreview",
  "references": {
    "http%3A//developer%2Emicrosoft%2Ecom":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "previewPriority": " !",
      "type": "Other"
    },
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "previewPriority": "  !!",
    },
    "http%3A//www%2Ebing%2Ecom": null
  },
  "checklist": {
    "95e27074-6c4a-447a-aa24-9d718a0b86fa":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "title": "Update task details",
      "ischecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="36cee-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="36cee-155">Response</span></span>
<span data-ttu-id="36cee-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36cee-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1793

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "8599273",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "http%3A//developer%2Emicrosoft%2Ecom": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "type": "Other",
      "previewPriority": "90727736",
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
      "isChecked": true,
      "title": "Try reading task details",
      "orderHint": "a93c93c5^",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "95e27074-6c4a-447a-aa24-9d718a0b86f": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Update task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
