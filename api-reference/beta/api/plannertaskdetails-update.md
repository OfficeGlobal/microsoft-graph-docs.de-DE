---
title: plannertaskdetails aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannertaskdetails**-Objekts.
ms.openlocfilehash: e0f3768b1f6afcbbda6b7467973cf829beb3a072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060664"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="21298-103">plannertaskdetails aktualisieren</span><span class="sxs-lookup"><span data-stu-id="21298-103">Update plannertaskdetails</span></span>

> <span data-ttu-id="21298-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21298-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21298-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21298-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21298-106">Dient zum Aktualisieren der Eigenschaften eines **plannertaskdetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="21298-106">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21298-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21298-107">Permissions</span></span>
<span data-ttu-id="21298-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21298-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21298-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21298-110">Permission type</span></span>      | <span data-ttu-id="21298-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21298-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21298-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21298-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21298-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21298-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21298-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21298-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21298-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21298-115">Not supported.</span></span>    |
|<span data-ttu-id="21298-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21298-116">Application</span></span> | <span data-ttu-id="21298-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21298-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21298-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21298-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="21298-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21298-119">Optional request headers</span></span>
| <span data-ttu-id="21298-120">Name</span><span class="sxs-lookup"><span data-stu-id="21298-120">Name</span></span>       | <span data-ttu-id="21298-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21298-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="21298-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21298-122">Authorization</span></span>  | <span data-ttu-id="21298-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21298-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21298-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="21298-125">If-Match</span></span>  | <span data-ttu-id="21298-p104">Letzter bekannter ETag-Wert für das zu aktualisierende **plannerTaskDetails**-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21298-p104">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21298-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21298-128">Request body</span></span>
<span data-ttu-id="21298-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="21298-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21298-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21298-132">Property</span></span>     | <span data-ttu-id="21298-133">Typ</span><span class="sxs-lookup"><span data-stu-id="21298-133">Type</span></span>   |<span data-ttu-id="21298-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21298-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21298-135">checklist</span><span class="sxs-lookup"><span data-stu-id="21298-135">checklist</span></span>|[<span data-ttu-id="21298-136">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="21298-136">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="21298-137">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="21298-137">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="21298-138">description</span><span class="sxs-lookup"><span data-stu-id="21298-138">description</span></span>|<span data-ttu-id="21298-139">String</span><span class="sxs-lookup"><span data-stu-id="21298-139">String</span></span>|<span data-ttu-id="21298-140">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="21298-140">Description of the task</span></span>|
|<span data-ttu-id="21298-141">previewType</span><span class="sxs-lookup"><span data-stu-id="21298-141">previewType</span></span>|<span data-ttu-id="21298-142">string</span><span class="sxs-lookup"><span data-stu-id="21298-142">string</span></span>|<span data-ttu-id="21298-p106">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="21298-p106">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="21298-146">references</span><span class="sxs-lookup"><span data-stu-id="21298-146">references</span></span>|[<span data-ttu-id="21298-147">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="21298-147">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="21298-148">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="21298-148">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="21298-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="21298-149">Response</span></span>

<span data-ttu-id="21298-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerTaskDetails](../resources/plannertaskdetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21298-150">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="21298-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="21298-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="21298-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21298-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21298-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21298-155">Request</span></span>
<span data-ttu-id="21298-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21298-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
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
      "isChecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="21298-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="21298-157">Response</span></span>
<span data-ttu-id="21298-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21298-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
