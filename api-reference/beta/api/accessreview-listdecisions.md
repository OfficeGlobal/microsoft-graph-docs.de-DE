---
title: Liste AccessReview Entscheidungen
description: In Azure AD Access Feature überprüft, die Entscheidungen eines AccessReview-Objekts abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927009"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="2bee4-103">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="2bee4-103">List accessReview decisions</span></span>

> <span data-ttu-id="2bee4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2bee4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bee4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2bee4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bee4-106">Abgerufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion werden die Entscheidungen eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2bee4-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="2bee4-107">Beachten Sie, dass sich wiederholenden Access Wiederholung wird eine `decisions` Beziehung.</span><span class="sxs-lookup"><span data-stu-id="2bee4-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="2bee4-108">Stattdessen muss der Aufrufer navigieren die `instance` Beziehung zu suchen ein `accessReview` -Objekt für eine aktuelle oder frühere Instanz der Überprüfung Access.</span><span class="sxs-lookup"><span data-stu-id="2bee4-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bee4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2bee4-109">Permissions</span></span>
<span data-ttu-id="2bee4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bee4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bee4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2bee4-112">Permission type</span></span>                        | <span data-ttu-id="2bee4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2bee4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bee4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2bee4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bee4-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="2bee4-115"></span></span>  <span data-ttu-id="2bee4-116">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="2bee4-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="2bee4-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2bee4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bee4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bee4-118">Not supported.</span></span> |
|<span data-ttu-id="2bee4-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2bee4-119">Application</span></span>                            | <span data-ttu-id="2bee4-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bee4-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bee4-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bee4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="2bee4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2bee4-122">Request headers</span></span>
| <span data-ttu-id="2bee4-123">Name</span><span class="sxs-lookup"><span data-stu-id="2bee4-123">Name</span></span>         | <span data-ttu-id="2bee4-124">Typ</span><span class="sxs-lookup"><span data-stu-id="2bee4-124">Type</span></span>        | <span data-ttu-id="2bee4-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bee4-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2bee4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bee4-126">Authorization</span></span> | <span data-ttu-id="2bee4-127">string</span><span class="sxs-lookup"><span data-stu-id="2bee4-127">string</span></span> | <span data-ttu-id="2bee4-128">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="2bee4-128">Bearer \{token\}.</span></span> <span data-ttu-id="2bee4-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2bee4-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bee4-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2bee4-130">Request body</span></span>
<span data-ttu-id="2bee4-131">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="2bee4-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="2bee4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bee4-132">Response</span></span>
<span data-ttu-id="2bee4-133">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [AccessReviewDecision](../resources/accessreviewdecision.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2bee4-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bee4-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2bee4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bee4-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bee4-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="2bee4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bee4-136">Response</span></span>
><span data-ttu-id="2bee4-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2bee4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2bee4-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2bee4-139">See also</span></span>

| <span data-ttu-id="2bee4-140">Methode</span><span class="sxs-lookup"><span data-stu-id="2bee4-140">Method</span></span>           | <span data-ttu-id="2bee4-141">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2bee4-141">Return Type</span></span>    |<span data-ttu-id="2bee4-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bee4-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2bee4-143">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="2bee4-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="2bee4-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="2bee4-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="2bee4-145">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="2bee4-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="2bee4-146">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="2bee4-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="2bee4-147">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2bee4-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="2bee4-148">Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="2bee4-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="2bee4-149">AccessReview Erinnerung senden</span><span class="sxs-lookup"><span data-stu-id="2bee4-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="2bee4-150">Keine.</span><span class="sxs-lookup"><span data-stu-id="2bee4-150">None.</span></span>   |   <span data-ttu-id="2bee4-151">Senden Sie eine Erinnerung an die Bearbeiter ein AccessReview.</span><span class="sxs-lookup"><span data-stu-id="2bee4-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="2bee4-152">AccessReview beenden</span><span class="sxs-lookup"><span data-stu-id="2bee4-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="2bee4-153">Keine.</span><span class="sxs-lookup"><span data-stu-id="2bee4-153">None.</span></span>   |   <span data-ttu-id="2bee4-154">Beenden einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="2bee4-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="2bee4-155">AccessReview Entscheidungen zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="2bee4-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="2bee4-156">Keine.</span><span class="sxs-lookup"><span data-stu-id="2bee4-156">None.</span></span>   |   <span data-ttu-id="2bee4-157">Setzen Sie die Entscheidungen in einer laufenden AccessReview zurück.</span><span class="sxs-lookup"><span data-stu-id="2bee4-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="2bee4-158">Anwenden von AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="2bee4-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="2bee4-159">Keine.</span><span class="sxs-lookup"><span data-stu-id="2bee4-159">None.</span></span>   |   <span data-ttu-id="2bee4-160">Gelten Sie die Entscheidungen aus einer abgeschlossenen AccessReview.</span><span class="sxs-lookup"><span data-stu-id="2bee4-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
