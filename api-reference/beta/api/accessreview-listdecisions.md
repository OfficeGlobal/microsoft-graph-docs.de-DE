---
title: Liste AccessReview Entscheidungen
description: In Azure AD Access Feature überprüft, die Entscheidungen eines AccessReview-Objekts abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521796"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="a7bb0-103">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="a7bb0-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7bb0-104">Abgerufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion werden die Entscheidungen eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a7bb0-105">Beachten Sie, dass sich wiederholenden Access Wiederholung wird eine `decisions` Beziehung.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="a7bb0-106">Stattdessen muss der Aufrufer navigieren die `instance` Beziehung zu suchen ein `accessReview` -Objekt für eine aktuelle oder frühere Instanz der Überprüfung Access.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7bb0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a7bb0-107">Permissions</span></span>
<span data-ttu-id="a7bb0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7bb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7bb0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7bb0-110">Permission type</span></span>                        | <span data-ttu-id="a7bb0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7bb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7bb0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7bb0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7bb0-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-113"></span></span>  <span data-ttu-id="a7bb0-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="a7bb0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7bb0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7bb0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7bb0-116">Not supported.</span></span> |
|<span data-ttu-id="a7bb0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-117">Application</span></span>                            | <span data-ttu-id="a7bb0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7bb0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7bb0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="a7bb0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7bb0-120">Request headers</span></span>
| <span data-ttu-id="a7bb0-121">Name</span><span class="sxs-lookup"><span data-stu-id="a7bb0-121">Name</span></span>         | <span data-ttu-id="a7bb0-122">Typ</span><span class="sxs-lookup"><span data-stu-id="a7bb0-122">Type</span></span>        | <span data-ttu-id="a7bb0-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a7bb0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7bb0-124">Authorization</span></span> | <span data-ttu-id="a7bb0-125">string</span><span class="sxs-lookup"><span data-stu-id="a7bb0-125">string</span></span> | <span data-ttu-id="a7bb0-126">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="a7bb0-126">Bearer \{token\}.</span></span> <span data-ttu-id="a7bb0-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7bb0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7bb0-128">Request body</span></span>
<span data-ttu-id="a7bb0-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a7bb0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7bb0-130">Response</span></span>
<span data-ttu-id="a7bb0-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [AccessReviewDecision](../resources/accessreviewdecision.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7bb0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7bb0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7bb0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="a7bb0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7bb0-134">Response</span></span>
><span data-ttu-id="a7bb0-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="a7bb0-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a7bb0-137">See also</span></span>

| <span data-ttu-id="a7bb0-138">Methode</span><span class="sxs-lookup"><span data-stu-id="a7bb0-138">Method</span></span>           | <span data-ttu-id="a7bb0-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a7bb0-139">Return Type</span></span>    |<span data-ttu-id="a7bb0-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7bb0-141">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="a7bb0-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a7bb0-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="a7bb0-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a7bb0-143">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a7bb0-144">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="a7bb0-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="a7bb0-145">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a7bb0-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="a7bb0-146">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a7bb0-147">AccessReview Erinnerung senden</span><span class="sxs-lookup"><span data-stu-id="a7bb0-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="a7bb0-148">Keine.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-148">None.</span></span>   |   <span data-ttu-id="a7bb0-149">Senden Sie eine Erinnerung an die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a7bb0-150">AccessReview beenden</span><span class="sxs-lookup"><span data-stu-id="a7bb0-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="a7bb0-151">Keine.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-151">None.</span></span>   |   <span data-ttu-id="a7bb0-152">Beenden einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="a7bb0-153">AccessReview Entscheidungen zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="a7bb0-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="a7bb0-154">Keine.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-154">None.</span></span>   |   <span data-ttu-id="a7bb0-155">Setzen Sie die Entscheidungen in einer laufenden AccessReview zurück.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="a7bb0-156">Anwenden von AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="a7bb0-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="a7bb0-157">Keine.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-157">None.</span></span>   |   <span data-ttu-id="a7bb0-158">Gelten Sie die Entscheidungen aus einer abgeschlossenen AccessReview.</span><span class="sxs-lookup"><span data-stu-id="a7bb0-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
