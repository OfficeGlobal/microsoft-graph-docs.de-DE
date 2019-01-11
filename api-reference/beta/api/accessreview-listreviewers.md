---
title: Liste AccessReview Bearbeiter
description: In Azure AD Access Feature überprüft, die Bearbeiter eines AccessReview-Objekts abrufen.
localization_priority: Normal
ms.openlocfilehash: 042887944902be9a603ae0581835c8d55355f8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829372"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="8ead2-103">Liste AccessReview Bearbeiter</span><span class="sxs-lookup"><span data-stu-id="8ead2-103">List accessReview reviewers</span></span>

> <span data-ttu-id="8ead2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ead2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ead2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ead2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ead2-106">Rufen Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Bearbeiter eines [AccessReview](../resources/accessreview.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="8ead2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ead2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ead2-107">Permissions</span></span>
<span data-ttu-id="8ead2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ead2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ead2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ead2-110">Permission type</span></span>                        | <span data-ttu-id="8ead2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ead2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ead2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ead2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ead2-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="8ead2-113"></span></span>  <span data-ttu-id="8ead2-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="8ead2-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="8ead2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ead2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ead2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ead2-116">Not supported.</span></span> |
|<span data-ttu-id="8ead2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ead2-117">Application</span></span>                            | <span data-ttu-id="8ead2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ead2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ead2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ead2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="8ead2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ead2-120">Request headers</span></span>
| <span data-ttu-id="8ead2-121">Name</span><span class="sxs-lookup"><span data-stu-id="8ead2-121">Name</span></span>         | <span data-ttu-id="8ead2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="8ead2-122">Type</span></span>        | <span data-ttu-id="8ead2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ead2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8ead2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ead2-124">Authorization</span></span> | <span data-ttu-id="8ead2-125">string</span><span class="sxs-lookup"><span data-stu-id="8ead2-125">string</span></span> | <span data-ttu-id="8ead2-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="8ead2-126">Bearer \{token\}.</span></span> <span data-ttu-id="8ead2-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ead2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ead2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ead2-128">Request body</span></span>
<span data-ttu-id="8ead2-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="8ead2-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="8ead2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ead2-130">Response</span></span>
<span data-ttu-id="8ead2-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein Array von Objekten im Antworttext [Benutzeridentität](../resources/useridentity.md) .</span><span class="sxs-lookup"><span data-stu-id="8ead2-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ead2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ead2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ead2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ead2-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="8ead2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ead2-134">Response</span></span>
><span data-ttu-id="8ead2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8ead2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8ead2-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="8ead2-137">See also</span></span>

| <span data-ttu-id="8ead2-138">Methode</span><span class="sxs-lookup"><span data-stu-id="8ead2-138">Method</span></span>           | <span data-ttu-id="8ead2-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8ead2-139">Return Type</span></span>    |<span data-ttu-id="8ead2-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ead2-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ead2-141">Abrufen von accessReview</span><span class="sxs-lookup"><span data-stu-id="8ead2-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="8ead2-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="8ead2-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="8ead2-143">Abrufen einer Access-Überprüfung.</span><span class="sxs-lookup"><span data-stu-id="8ead2-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="8ead2-144">AccessReview Bearbeiter hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8ead2-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="8ead2-145">Keine.</span><span class="sxs-lookup"><span data-stu-id="8ead2-145">None.</span></span>   |   <span data-ttu-id="8ead2-146">Fügen Sie einem Bearbeiter ein AccessReview hinzu.</span><span class="sxs-lookup"><span data-stu-id="8ead2-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="8ead2-147">AccessReview Reviewer entfernen</span><span class="sxs-lookup"><span data-stu-id="8ead2-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="8ead2-148">Keine.</span><span class="sxs-lookup"><span data-stu-id="8ead2-148">None.</span></span> |   <span data-ttu-id="8ead2-149">Entfernen Sie einen Prüfer aus einer AccessReview.</span><span class="sxs-lookup"><span data-stu-id="8ead2-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
