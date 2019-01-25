---
title: Meine AccessReview Entscheidungen auflisten
description: In Azure AD Access Feature überprüft, die Entscheidungen eines AccessReview-Objekts für den aufrufenden Benutzer als Reviewer abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525325"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="daebe-103">Meine AccessReview Entscheidungen auflisten</span><span class="sxs-lookup"><span data-stu-id="daebe-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daebe-104">Abgerufen Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature werden die Entscheidungen eines [AccessReview](../resources/accessreview.md) -Objekts für den aufrufenden Benutzer als Reviewer.</span><span class="sxs-lookup"><span data-stu-id="daebe-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="daebe-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="daebe-105">Permissions</span></span>
<span data-ttu-id="daebe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daebe-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="daebe-108">Permission type</span></span>                        | <span data-ttu-id="daebe-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="daebe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="daebe-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="daebe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="daebe-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="daebe-111"></span></span>  <span data-ttu-id="daebe-112">Der Benutzer angemeldet muss auch zum Lesen von dieser bestimmten Access Überprüfung zulässig sein.</span><span class="sxs-lookup"><span data-stu-id="daebe-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="daebe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="daebe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daebe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="daebe-114">Not supported.</span></span> |
|<span data-ttu-id="daebe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="daebe-115">Application</span></span>                            | <span data-ttu-id="daebe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="daebe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="daebe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="daebe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="daebe-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="daebe-118">Request headers</span></span>
| <span data-ttu-id="daebe-119">Name</span><span class="sxs-lookup"><span data-stu-id="daebe-119">Name</span></span>         | <span data-ttu-id="daebe-120">Typ</span><span class="sxs-lookup"><span data-stu-id="daebe-120">Type</span></span>        | <span data-ttu-id="daebe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daebe-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="daebe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="daebe-122">Authorization</span></span> | <span data-ttu-id="daebe-123">string</span><span class="sxs-lookup"><span data-stu-id="daebe-123">string</span></span> | <span data-ttu-id="daebe-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="daebe-124">Bearer \{token\}.</span></span> <span data-ttu-id="daebe-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="daebe-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="daebe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="daebe-126">Request body</span></span>
<span data-ttu-id="daebe-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="daebe-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="daebe-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="daebe-128">Response</span></span>
<span data-ttu-id="daebe-129">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [AccessReviewDecision](../resources/accessreviewdecision.md) -Objekten im Antworttext, für die der aufrufende Benutzer einer zugewiesenen Reviewer ist.</span><span class="sxs-lookup"><span data-stu-id="daebe-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="daebe-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="daebe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="daebe-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="daebe-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="daebe-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="daebe-132">Response</span></span>
><span data-ttu-id="daebe-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="daebe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="daebe-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="daebe-135">See also</span></span>

| <span data-ttu-id="daebe-136">Methode</span><span class="sxs-lookup"><span data-stu-id="daebe-136">Method</span></span>           | <span data-ttu-id="daebe-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="daebe-137">Return Type</span></span>    |<span data-ttu-id="daebe-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daebe-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="daebe-139">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="daebe-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="daebe-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="daebe-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="daebe-141">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="daebe-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="daebe-142">Liste AccessReview Entscheidungen</span><span class="sxs-lookup"><span data-stu-id="daebe-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="daebe-143">[AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="daebe-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="daebe-144">Rufen Sie alle Entscheidungen von einer AccessReview ab.</span><span class="sxs-lookup"><span data-stu-id="daebe-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
