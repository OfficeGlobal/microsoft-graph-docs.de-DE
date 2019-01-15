---
title: Abrufen von accessReview
description: 'In Azure AD Access Feature überprüft, ein AccessReview-Objekt abrufen.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a13776b9aa215d752797b6ba2de2f477660ed31d
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016660"
---
# <a name="get-accessreview"></a><span data-ttu-id="e3664-103">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="e3664-103">Get accessReview</span></span>

> <span data-ttu-id="e3664-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3664-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3664-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3664-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3664-106">Rufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="e3664-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="e3664-107">Verwenden Sie zum Abrufen der Bearbeiter die Überprüfung Access die [Liste AccessReview Bearbeiter](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="e3664-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="e3664-108">Verwenden Sie zum Abrufen der Entscheidungen der Access Überprüfung der [Liste AccessReview Entscheidungen](accessreview-listdecisions.md) -API oder der [Liste Meine AccessReview Entscheidungen](accessreview-listmydecisions.md) -API.</span><span class="sxs-lookup"><span data-stu-id="e3664-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="e3664-109">Ist dies eine periodische Access-Überprüfung, und verwenden Sie dann die `instances` Beziehung zum Abrufen einer [AccessReview](../resources/accessreview.md) -Auflistung des aktuellen und zukünftigen Instanzen der Access Überprüfung der Vergangenheit.</span><span class="sxs-lookup"><span data-stu-id="e3664-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3664-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3664-110">Permissions</span></span>
<span data-ttu-id="e3664-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3664-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3664-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3664-113">Permission type</span></span>                        | <span data-ttu-id="e3664-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3664-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3664-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3664-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3664-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e3664-116"></span></span>  <span data-ttu-id="e3664-117">Der angemeldeten Benutzer muss auch in ein Verzeichnis Rolle sein, die ermöglicht eine Überprüfung Access lesen oder als ein Prüfer für die Überprüfung Access zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e3664-117">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="e3664-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3664-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3664-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3664-119">Not supported.</span></span> |
|<span data-ttu-id="e3664-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3664-120">Application</span></span>                            | <span data-ttu-id="e3664-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3664-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3664-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3664-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="e3664-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3664-123">Request headers</span></span>
| <span data-ttu-id="e3664-124">Name</span><span class="sxs-lookup"><span data-stu-id="e3664-124">Name</span></span>         | <span data-ttu-id="e3664-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e3664-125">Type</span></span>        | <span data-ttu-id="e3664-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3664-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3664-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3664-127">Authorization</span></span> | <span data-ttu-id="e3664-128">String</span><span class="sxs-lookup"><span data-stu-id="e3664-128">string</span></span> | <span data-ttu-id="e3664-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="e3664-129">Bearer \{token\}.</span></span> <span data-ttu-id="e3664-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3664-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3664-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3664-131">Request body</span></span>
<span data-ttu-id="e3664-132">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e3664-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e3664-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3664-133">Response</span></span>
<span data-ttu-id="e3664-134">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e3664-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3664-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3664-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3664-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3664-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="e3664-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3664-137">Response</span></span>
><span data-ttu-id="e3664-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e3664-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e3664-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e3664-140">See also</span></span>

| <span data-ttu-id="e3664-141">Methode</span><span class="sxs-lookup"><span data-stu-id="e3664-141">Method</span></span>           | <span data-ttu-id="e3664-142">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e3664-142">Return Type</span></span>    |<span data-ttu-id="e3664-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3664-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3664-144">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="e3664-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="e3664-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="e3664-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e3664-146">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="e3664-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="e3664-147">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="e3664-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="e3664-148">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e3664-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="e3664-149">Liste ProgramControls in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3664-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="e3664-150">Liste AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="e3664-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="e3664-151">[Benutzeridentität](../resources/useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e3664-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="e3664-152">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="e3664-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="e3664-153">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="e3664-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="e3664-154">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e3664-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="e3664-155">Rufen Sie die Entscheidungen des ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="e3664-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="e3664-156">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="e3664-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="e3664-157">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e3664-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="e3664-158">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="e3664-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
