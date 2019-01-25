---
title: Liste AccessReview Bearbeiter
description: In Azure AD Access Feature überprüft, die Bearbeiter eines AccessReview-Objekts abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529278"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="53f20-103">Liste AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="53f20-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53f20-104">Rufen Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Bearbeiter eines [AccessReview](../resources/accessreview.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="53f20-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53f20-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53f20-105">Permissions</span></span>
<span data-ttu-id="53f20-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f20-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53f20-108">Permission type</span></span>                        | <span data-ttu-id="53f20-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53f20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53f20-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53f20-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53f20-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="53f20-111"></span></span>  <span data-ttu-id="53f20-112">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="53f20-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="53f20-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53f20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f20-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53f20-114">Not supported.</span></span> |
|<span data-ttu-id="53f20-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53f20-115">Application</span></span>                            | <span data-ttu-id="53f20-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53f20-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53f20-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53f20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="53f20-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53f20-118">Request headers</span></span>
| <span data-ttu-id="53f20-119">Name</span><span class="sxs-lookup"><span data-stu-id="53f20-119">Name</span></span>         | <span data-ttu-id="53f20-120">Typ</span><span class="sxs-lookup"><span data-stu-id="53f20-120">Type</span></span>        | <span data-ttu-id="53f20-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53f20-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53f20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f20-122">Authorization</span></span> | <span data-ttu-id="53f20-123">string</span><span class="sxs-lookup"><span data-stu-id="53f20-123">string</span></span> | <span data-ttu-id="53f20-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="53f20-124">Bearer \{token\}.</span></span> <span data-ttu-id="53f20-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53f20-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53f20-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53f20-126">Request body</span></span>
<span data-ttu-id="53f20-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="53f20-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="53f20-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="53f20-128">Response</span></span>
<span data-ttu-id="53f20-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein Array von Objekten im Antworttext [Benutzeridentität](../resources/useridentity.md) .</span><span class="sxs-lookup"><span data-stu-id="53f20-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53f20-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53f20-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53f20-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53f20-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="53f20-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="53f20-132">Response</span></span>
><span data-ttu-id="53f20-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="53f20-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="53f20-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="53f20-135">See also</span></span>

| <span data-ttu-id="53f20-136">Methode</span><span class="sxs-lookup"><span data-stu-id="53f20-136">Method</span></span>           | <span data-ttu-id="53f20-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="53f20-137">Return Type</span></span>    |<span data-ttu-id="53f20-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53f20-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53f20-139">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="53f20-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="53f20-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="53f20-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="53f20-141">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="53f20-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="53f20-142">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="53f20-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="53f20-143">Keine.</span><span class="sxs-lookup"><span data-stu-id="53f20-143">None.</span></span>   |   <span data-ttu-id="53f20-144">Fügen Sie einem Bearbeiter ein AccessReview hinzu.</span><span class="sxs-lookup"><span data-stu-id="53f20-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="53f20-145">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="53f20-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="53f20-146">Keine.</span><span class="sxs-lookup"><span data-stu-id="53f20-146">None.</span></span> |   <span data-ttu-id="53f20-147">Entfernen Sie einen Prüfer aus einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="53f20-147">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
