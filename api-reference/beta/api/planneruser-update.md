---
title: PlannerUser aktualisieren
description: Aktualisieren Sie die Eigenschaften eines PlannerUser-Objekts. Verwenden Sie diese Operation zum Hinzufügen oder Entfernen von Plänen aus der Liste eines Benutzers bevorzugten Pläne und um anzugeben, die den Benutzer plant wurde kürzlich angezeigt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508923"
---
# <a name="update-planneruser"></a><span data-ttu-id="4604e-104">PlannerUser aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4604e-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4604e-105">Aktualisieren Sie die Eigenschaften eines [PlannerUser](../resources/planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4604e-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="4604e-106">Verwenden Sie diese Operation zum Hinzufügen oder Entfernen von Plänen aus der Liste eines Benutzers bevorzugten Pläne und um anzugeben, die den Benutzer plant wurde kürzlich angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4604e-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="4604e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4604e-107">Permissions</span></span>
<span data-ttu-id="4604e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4604e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4604e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4604e-110">Permission type</span></span>      | <span data-ttu-id="4604e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4604e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4604e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4604e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4604e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4604e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4604e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4604e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4604e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4604e-115">Not supported.</span></span>    |
|<span data-ttu-id="4604e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4604e-116">Application</span></span> | <span data-ttu-id="4604e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4604e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4604e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4604e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="4604e-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4604e-119">Optional request headers</span></span>
| <span data-ttu-id="4604e-120">Name</span><span class="sxs-lookup"><span data-stu-id="4604e-120">Name</span></span>       | <span data-ttu-id="4604e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4604e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4604e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4604e-122">Authorization</span></span>  | <span data-ttu-id="4604e-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4604e-p104">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="4604e-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="4604e-125">If-Match</span></span>  | <span data-ttu-id="4604e-126">Letzte bekannten ETag-Wert für die **PlannerUser** aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="4604e-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="4604e-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4604e-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4604e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4604e-128">Request body</span></span>
<span data-ttu-id="4604e-129">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4604e-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4604e-130">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="4604e-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4604e-131">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="4604e-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4604e-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4604e-132">Property</span></span>     | <span data-ttu-id="4604e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4604e-133">Type</span></span>   |<span data-ttu-id="4604e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4604e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4604e-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="4604e-135">favoritePlanReferences</span></span>|[<span data-ttu-id="4604e-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4604e-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="4604e-137">Änderungen an der Auflistung, die die Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="4604e-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="4604e-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="4604e-138">recentPlanReferences</span></span>|[<span data-ttu-id="4604e-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4604e-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="4604e-140">Änderungen an der Auflistung, die die Verweise auf die Pläne, die der Benutzer zuletzt aufgerufen wurde.</span><span class="sxs-lookup"><span data-stu-id="4604e-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="4604e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4604e-141">Response</span></span>
<span data-ttu-id="4604e-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [PlannerUser](../resources/planneruser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4604e-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="4604e-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4604e-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="4604e-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4604e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4604e-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4604e-147">Request</span></span>
<span data-ttu-id="4604e-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4604e-148">The following is an example of the request.</span></span> <span data-ttu-id="4604e-149">Diese Anforderung des Plans "Nächsten Version Diskussion" mit der ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" als Favoriten des Benutzers hinzugefügt und Plan mit der ID "7oTB5aMIAE2rVo 1N L7RmQAGX2q" aus der Liste der bevorzugten Pläne entfernt.</span><span class="sxs-lookup"><span data-stu-id="4604e-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="4604e-150">Darüber hinaus wird die Uhrzeit der letzten Ansicht des Plans "jd8S5gOaFk2S8aWCIAJz42QAAxtD" aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4604e-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="4604e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="4604e-151">Response</span></span>
<span data-ttu-id="4604e-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4604e-152">The following is an example of the response.</span></span> 

><span data-ttu-id="4604e-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4604e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
