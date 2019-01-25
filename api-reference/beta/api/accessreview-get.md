---
title: Abrufen von accessReview
description: 'In Azure AD Access Feature überprüft, ein AccessReview-Objekt abrufen.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529145"
---
# <a name="get-accessreview"></a><span data-ttu-id="7213c-103">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="7213c-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7213c-104">Rufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="7213c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="7213c-105">Verwenden Sie zum Abrufen der Bearbeiter die Überprüfung Access die [Liste AccessReview Bearbeiter](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="7213c-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="7213c-106">Verwenden Sie zum Abrufen der Entscheidungen der Access Überprüfung der [Liste AccessReview Entscheidungen](accessreview-listdecisions.md) -API oder der [Liste Meine AccessReview Entscheidungen](accessreview-listmydecisions.md) -API.</span><span class="sxs-lookup"><span data-stu-id="7213c-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="7213c-107">Ist dies eine periodische Access-Überprüfung, und verwenden Sie dann die `instances` Beziehung zum Abrufen einer [AccessReview](../resources/accessreview.md) -Auflistung des aktuellen und zukünftigen Instanzen der Access Überprüfung der Vergangenheit.</span><span class="sxs-lookup"><span data-stu-id="7213c-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="7213c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7213c-108">Permissions</span></span>
<span data-ttu-id="7213c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7213c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7213c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7213c-111">Permission type</span></span>                        | <span data-ttu-id="7213c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7213c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7213c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7213c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7213c-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="7213c-114"></span></span>  <span data-ttu-id="7213c-115">Der angemeldeten Benutzer muss auch in ein Verzeichnis Rolle sein, die ermöglicht eine Überprüfung Access lesen oder als ein Prüfer für die Überprüfung Access zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="7213c-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="7213c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7213c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7213c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7213c-117">Not supported.</span></span> |
|<span data-ttu-id="7213c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7213c-118">Application</span></span>                            | <span data-ttu-id="7213c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7213c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7213c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7213c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="7213c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7213c-121">Request headers</span></span>
| <span data-ttu-id="7213c-122">Name</span><span class="sxs-lookup"><span data-stu-id="7213c-122">Name</span></span>         | <span data-ttu-id="7213c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7213c-123">Type</span></span>        | <span data-ttu-id="7213c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7213c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7213c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7213c-125">Authorization</span></span> | <span data-ttu-id="7213c-126">string</span><span class="sxs-lookup"><span data-stu-id="7213c-126">string</span></span> | <span data-ttu-id="7213c-127">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="7213c-127">Bearer \{token\}.</span></span> <span data-ttu-id="7213c-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7213c-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7213c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7213c-129">Request body</span></span>
<span data-ttu-id="7213c-130">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="7213c-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7213c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7213c-131">Response</span></span>
<span data-ttu-id="7213c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7213c-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7213c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7213c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7213c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7213c-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="7213c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7213c-135">Response</span></span>
><span data-ttu-id="7213c-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7213c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="7213c-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7213c-138">See also</span></span>

| <span data-ttu-id="7213c-139">Methode</span><span class="sxs-lookup"><span data-stu-id="7213c-139">Method</span></span>           | <span data-ttu-id="7213c-140">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7213c-140">Return Type</span></span>    |<span data-ttu-id="7213c-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7213c-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7213c-142">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="7213c-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="7213c-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="7213c-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="7213c-144">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7213c-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="7213c-145">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="7213c-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="7213c-146">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7213c-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="7213c-147">Liste ProgramControls in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7213c-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="7213c-148">Liste AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="7213c-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="7213c-149">[Benutzeridentität](../resources/useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7213c-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="7213c-150">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7213c-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="7213c-151">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="7213c-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="7213c-152">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7213c-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7213c-153">Rufen Sie die Entscheidungen des ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7213c-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="7213c-154">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="7213c-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="7213c-155">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7213c-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7213c-156">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7213c-156">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
