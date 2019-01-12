---
title: Meine AccessReview Entscheidungen auflisten
description: In Azure AD Access Feature überprüft, die Entscheidungen eines AccessReview-Objekts für den aufrufenden Benutzer als Reviewer abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 037b916bca45c74d1918b45e4e9e21b685bd8ae0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941499"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="a1be2-103">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="a1be2-103">List my accessReview decisions</span></span>

> <span data-ttu-id="a1be2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a1be2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1be2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1be2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1be2-106">Abgerufen Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature werden die Entscheidungen eines [AccessReview](../resources/accessreview.md) -Objekts für den aufrufenden Benutzer als Reviewer.</span><span class="sxs-lookup"><span data-stu-id="a1be2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1be2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a1be2-107">Permissions</span></span>
<span data-ttu-id="a1be2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1be2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1be2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1be2-110">Permission type</span></span>                        | <span data-ttu-id="a1be2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1be2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1be2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1be2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1be2-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a1be2-113"></span></span>  <span data-ttu-id="a1be2-114">Der Benutzer angemeldet muss auch zum Lesen von dieser bestimmten Access Überprüfung zulässig sein.</span><span class="sxs-lookup"><span data-stu-id="a1be2-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="a1be2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1be2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1be2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1be2-116">Not supported.</span></span> |
|<span data-ttu-id="a1be2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1be2-117">Application</span></span>                            | <span data-ttu-id="a1be2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1be2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1be2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1be2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="a1be2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1be2-120">Request headers</span></span>
| <span data-ttu-id="a1be2-121">Name</span><span class="sxs-lookup"><span data-stu-id="a1be2-121">Name</span></span>         | <span data-ttu-id="a1be2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="a1be2-122">Type</span></span>        | <span data-ttu-id="a1be2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1be2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a1be2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1be2-124">Authorization</span></span> | <span data-ttu-id="a1be2-125">string</span><span class="sxs-lookup"><span data-stu-id="a1be2-125">string</span></span> | <span data-ttu-id="a1be2-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="a1be2-126">Bearer \{token\}.</span></span> <span data-ttu-id="a1be2-127">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="a1be2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1be2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1be2-128">Request body</span></span>
<span data-ttu-id="a1be2-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="a1be2-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a1be2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1be2-130">Response</span></span>
<span data-ttu-id="a1be2-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [AccessReviewDecision](../resources/accessreviewdecision.md) -Objekten im Antworttext, für die der aufrufende Benutzer einer zugewiesenen Reviewer ist.</span><span class="sxs-lookup"><span data-stu-id="a1be2-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="a1be2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1be2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1be2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1be2-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="a1be2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1be2-134">Response</span></span>
><span data-ttu-id="a1be2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a1be2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a1be2-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a1be2-137">See also</span></span>

| <span data-ttu-id="a1be2-138">Methode</span><span class="sxs-lookup"><span data-stu-id="a1be2-138">Method</span></span>           | <span data-ttu-id="a1be2-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a1be2-139">Return Type</span></span>    |<span data-ttu-id="a1be2-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1be2-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1be2-141">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="a1be2-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a1be2-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="a1be2-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a1be2-143">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="a1be2-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a1be2-144">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="a1be2-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="a1be2-145">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a1be2-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="a1be2-146">Rufen Sie alle Entscheidungen von einer AccessReview ab.</span><span class="sxs-lookup"><span data-stu-id="a1be2-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
