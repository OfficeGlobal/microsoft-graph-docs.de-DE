---
title: PlannerUser aktualisieren
description: Aktualisieren Sie die Eigenschaften eines PlannerUser-Objekts. Verwenden Sie diese Operation zum Hinzufügen oder Entfernen von Plänen aus der Liste eines Benutzers bevorzugten Pläne und um anzugeben, die den Benutzer plant wurde kürzlich angezeigt.
localization_priority: Normal
ms.openlocfilehash: ae09deff65c5de08d80e34140abacd43d43a94b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889054"
---
# <a name="update-planneruser"></a><span data-ttu-id="528f6-104">PlannerUser aktualisieren</span><span class="sxs-lookup"><span data-stu-id="528f6-104">Update plannerUser</span></span>

> <span data-ttu-id="528f6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="528f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="528f6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="528f6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="528f6-107">Aktualisieren Sie die Eigenschaften eines [PlannerUser](../resources/planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="528f6-107">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="528f6-108">Verwenden Sie diese Operation zum Hinzufügen oder Entfernen von Plänen aus der Liste eines Benutzers bevorzugten Pläne und um anzugeben, die den Benutzer plant wurde kürzlich angezeigt.</span><span class="sxs-lookup"><span data-stu-id="528f6-108">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="528f6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="528f6-109">Permissions</span></span>
<span data-ttu-id="528f6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="528f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="528f6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="528f6-112">Permission type</span></span>      | <span data-ttu-id="528f6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="528f6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="528f6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="528f6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="528f6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="528f6-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="528f6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="528f6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="528f6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="528f6-117">Not supported.</span></span>    |
|<span data-ttu-id="528f6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="528f6-118">Application</span></span> | <span data-ttu-id="528f6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="528f6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="528f6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="528f6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="528f6-121">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="528f6-121">Optional request headers</span></span>
| <span data-ttu-id="528f6-122">Name</span><span class="sxs-lookup"><span data-stu-id="528f6-122">Name</span></span>       | <span data-ttu-id="528f6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="528f6-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="528f6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="528f6-124">Authorization</span></span>  | <span data-ttu-id="528f6-p105">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="528f6-p105">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="528f6-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="528f6-127">If-Match</span></span>  | <span data-ttu-id="528f6-128">Letzte bekannten ETag-Wert für die **PlannerUser** aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="528f6-128">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="528f6-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="528f6-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="528f6-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="528f6-130">Request body</span></span>
<span data-ttu-id="528f6-131">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="528f6-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="528f6-132">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="528f6-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="528f6-133">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="528f6-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="528f6-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="528f6-134">Property</span></span>     | <span data-ttu-id="528f6-135">Typ</span><span class="sxs-lookup"><span data-stu-id="528f6-135">Type</span></span>   |<span data-ttu-id="528f6-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="528f6-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="528f6-137">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="528f6-137">favoritePlanReferences</span></span>|[<span data-ttu-id="528f6-138">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="528f6-138">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="528f6-139">Änderungen an der Auflistung, die die Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="528f6-139">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="528f6-140">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="528f6-140">recentPlanReferences</span></span>|[<span data-ttu-id="528f6-141">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="528f6-141">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="528f6-142">Änderungen an der Auflistung, die die Verweise auf die Pläne, die der Benutzer zuletzt aufgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="528f6-142">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="528f6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="528f6-143">Response</span></span>
<span data-ttu-id="528f6-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [PlannerUser](../resources/planneruser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="528f6-144">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="528f6-p108">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="528f6-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="528f6-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="528f6-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="528f6-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="528f6-149">Request</span></span>
<span data-ttu-id="528f6-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="528f6-150">The following is an example of the request.</span></span> <span data-ttu-id="528f6-151">Diese Anforderung des Plans "Nächsten Version Diskussion" mit der ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" als Favoriten des Benutzers hinzugefügt und Plan mit der ID "7oTB5aMIAE2rVo 1N L7RmQAGX2q" aus der Liste der bevorzugten Pläne entfernt.</span><span class="sxs-lookup"><span data-stu-id="528f6-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="528f6-152">Darüber hinaus wird die Uhrzeit der letzten Ansicht des Plans "jd8S5gOaFk2S8aWCIAJz42QAAxtD" aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="528f6-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a><span data-ttu-id="528f6-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="528f6-153">Response</span></span>
<span data-ttu-id="528f6-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="528f6-154">The following is an example of the response.</span></span> 

><span data-ttu-id="528f6-p110">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="528f6-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
