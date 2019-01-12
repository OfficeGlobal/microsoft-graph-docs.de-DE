---
title: Abrufen von accessReview
description: 'In Azure AD Access Feature überprüft, ein AccessReview-Objekt abrufen.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be946e07a7714dc744847d73ee49718237fac92e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926659"
---
# <a name="get-accessreview"></a><span data-ttu-id="92ae3-103">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="92ae3-103">Get accessReview</span></span>

> <span data-ttu-id="92ae3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92ae3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92ae3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92ae3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92ae3-106">Rufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="92ae3-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="92ae3-107">Verwenden Sie zum Abrufen der Bearbeiter die Überprüfung Access die [Liste AccessReview Bearbeiter](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="92ae3-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="92ae3-108">Verwenden Sie zum Abrufen der Entscheidungen der Access Überprüfung der [Liste AccessReview Entscheidungen](accessreview-listdecisions.md) -API oder der [Liste Meine AccessReview Entscheidungen](accessreview-listmydecisions.md) -API.</span><span class="sxs-lookup"><span data-stu-id="92ae3-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="92ae3-109">Ist dies eine periodische Access-Überprüfung, und verwenden Sie dann die `instances` Beziehung zum Abrufen einer [AccessReview](../resources/accessreview.md) -Auflistung des aktuellen und zukünftigen Instanzen der Access Überprüfung der Vergangenheit.</span><span class="sxs-lookup"><span data-stu-id="92ae3-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="92ae3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="92ae3-110">Permissions</span></span>
<span data-ttu-id="92ae3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ae3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ae3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92ae3-113">Permission type</span></span>                        | <span data-ttu-id="92ae3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92ae3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ae3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92ae3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="92ae3-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="92ae3-116"></span></span>  <span data-ttu-id="92ae3-117">Der Benutzer angemeldet muss auch in einer Rolle Directory ermöglicht eine Überprüfung Access lesen oder als ein Prüfer für die Überprüfung Access zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="92ae3-117">The signed in user must also be in a directory role which permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="92ae3-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92ae3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ae3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92ae3-119">Not supported.</span></span> |
|<span data-ttu-id="92ae3-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92ae3-120">Application</span></span>                            | <span data-ttu-id="92ae3-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92ae3-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92ae3-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92ae3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="92ae3-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92ae3-123">Request headers</span></span>
| <span data-ttu-id="92ae3-124">Name</span><span class="sxs-lookup"><span data-stu-id="92ae3-124">Name</span></span>         | <span data-ttu-id="92ae3-125">Typ</span><span class="sxs-lookup"><span data-stu-id="92ae3-125">Type</span></span>        | <span data-ttu-id="92ae3-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92ae3-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="92ae3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ae3-127">Authorization</span></span> | <span data-ttu-id="92ae3-128">string</span><span class="sxs-lookup"><span data-stu-id="92ae3-128">string</span></span> | <span data-ttu-id="92ae3-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="92ae3-129">Bearer \{token\}.</span></span> <span data-ttu-id="92ae3-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="92ae3-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92ae3-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92ae3-131">Request body</span></span>
<span data-ttu-id="92ae3-132">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="92ae3-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="92ae3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="92ae3-133">Response</span></span>
<span data-ttu-id="92ae3-134">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="92ae3-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ae3-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92ae3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92ae3-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92ae3-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="92ae3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="92ae3-137">Response</span></span>
><span data-ttu-id="92ae3-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="92ae3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "settings": {
        "reviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="92ae3-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="92ae3-140">See also</span></span>

| <span data-ttu-id="92ae3-141">Methode</span><span class="sxs-lookup"><span data-stu-id="92ae3-141">Method</span></span>           | <span data-ttu-id="92ae3-142">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="92ae3-142">Return Type</span></span>    |<span data-ttu-id="92ae3-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92ae3-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92ae3-144">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="92ae3-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="92ae3-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="92ae3-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="92ae3-146">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="92ae3-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="92ae3-147">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="92ae3-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="92ae3-148">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="92ae3-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="92ae3-149">Liste ProgramControls in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="92ae3-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="92ae3-150">Liste AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="92ae3-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="92ae3-151">[Benutzeridentität](../resources/useridentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="92ae3-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="92ae3-152">Rufen Sie die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="92ae3-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="92ae3-153">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="92ae3-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="92ae3-154">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="92ae3-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="92ae3-155">Rufen Sie die Entscheidungen des ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="92ae3-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="92ae3-156">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="92ae3-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="92ae3-157">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="92ae3-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="92ae3-158">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="92ae3-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
