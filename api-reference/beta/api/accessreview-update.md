---
title: AccessReview aktualisieren
description: In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um eine oder mehrere Eigenschaften ändern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e09219c1979f974b62f17c52163fc93b5d2d3c2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941355"
---
# <a name="update-accessreview"></a><span data-ttu-id="7730b-103">AccessReview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7730b-103">Update accessReview</span></span>

> <span data-ttu-id="7730b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7730b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7730b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7730b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7730b-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um eine oder mehrere Eigenschaften ändern.</span><span class="sxs-lookup"><span data-stu-id="7730b-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="7730b-107">Diese API ist nicht so ändern Sie die Bearbeiter oder Entscheidungen einer Überprüfung vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="7730b-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="7730b-108">Um die Bearbeiter ändern möchten, verwenden Sie die [AddReviewer](accessreview-addreviewer.md) oder [RemoveReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="7730b-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="7730b-109">Beenden einer bereits gestartet einmalige Überprüfung oder eine Instanz bereits gestartet eine periodische Überprüfung, frühzeitig und [Beenden](accessreview-stop.md) API verwenden, und um die Entscheidungen auf Ziel Zugriffsrechte Gruppe oder app anzuwenden verwenden Sie die [anwenden](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="7730b-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API, and to apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7730b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7730b-110">Permissions</span></span>
<span data-ttu-id="7730b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7730b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7730b-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7730b-113">Permission type</span></span>                        | <span data-ttu-id="7730b-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7730b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7730b-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7730b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7730b-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7730b-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7730b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7730b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7730b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7730b-118">Not supported.</span></span> |
|<span data-ttu-id="7730b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7730b-119">Application</span></span>                            | <span data-ttu-id="7730b-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7730b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7730b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7730b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="7730b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7730b-122">Request headers</span></span>
| <span data-ttu-id="7730b-123">Name</span><span class="sxs-lookup"><span data-stu-id="7730b-123">Name</span></span>         | <span data-ttu-id="7730b-124">Typ</span><span class="sxs-lookup"><span data-stu-id="7730b-124">Type</span></span>        | <span data-ttu-id="7730b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7730b-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7730b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7730b-126">Authorization</span></span> | <span data-ttu-id="7730b-127">string</span><span class="sxs-lookup"><span data-stu-id="7730b-127">string</span></span> | <span data-ttu-id="7730b-128">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="7730b-128">Bearer \{token\}.</span></span> <span data-ttu-id="7730b-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7730b-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7730b-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7730b-130">Request body</span></span>
<span data-ttu-id="7730b-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ein Parameter eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7730b-131">In the request body, supply a JSON representation of a parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="7730b-132">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="7730b-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="7730b-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7730b-133">Property</span></span>     | <span data-ttu-id="7730b-134">Typ</span><span class="sxs-lookup"><span data-stu-id="7730b-134">Type</span></span>        | <span data-ttu-id="7730b-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7730b-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="7730b-136">Der Name des Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7730b-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="7730b-137">Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="7730b-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="7730b-138">Dies muss ein Datum in der Zukunft sein.</span><span class="sxs-lookup"><span data-stu-id="7730b-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="7730b-139">Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden.</span><span class="sxs-lookup"><span data-stu-id="7730b-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="7730b-140">Dies muss mindestens einen Tag später als das Startdatum sein.</span><span class="sxs-lookup"><span data-stu-id="7730b-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="7730b-141">Die Beschreibung für die Bearbeiter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7730b-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="7730b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7730b-142">Response</span></span>
<span data-ttu-id="7730b-143">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `204, Accepted` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7730b-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7730b-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7730b-144">Example</span></span>

<span data-ttu-id="7730b-145">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7730b-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="7730b-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7730b-146">Request</span></span>
<span data-ttu-id="7730b-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der neuen Eigenschaften des [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7730b-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a><span data-ttu-id="7730b-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="7730b-148">Response</span></span>
><span data-ttu-id="7730b-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7730b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
