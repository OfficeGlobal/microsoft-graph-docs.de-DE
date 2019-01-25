---
title: AccessReview aktualisieren
description: In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um eine oder mehrere Eigenschaften ändern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524366"
---
# <a name="update-accessreview"></a><span data-ttu-id="790a9-103">AccessReview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="790a9-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="790a9-104">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um eine oder mehrere Eigenschaften ändern.</span><span class="sxs-lookup"><span data-stu-id="790a9-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="790a9-105">Diese API ist nicht so ändern Sie die Bearbeiter oder Entscheidungen einer Überprüfung vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="790a9-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="790a9-106">Um die Bearbeiter ändern möchten, verwenden Sie die [AddReviewer](accessreview-addreviewer.md) oder [RemoveReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="790a9-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="790a9-107">Verwenden Sie eine einmalige Überprüfung bei bereits gestartet, oder eine Instanz bereits gestartet periodische Wiederholung frühzeitig und, um beenden [Beenden](accessreview-stop.md) API.</span><span class="sxs-lookup"><span data-stu-id="790a9-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="790a9-108">Um die Entscheidungen über die Ziel-Gruppe oder app Zugriffsrechte anwenden möchten, verwenden Sie die [anwenden](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="790a9-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="790a9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="790a9-109">Permissions</span></span>
<span data-ttu-id="790a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790a9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="790a9-112">Permission type</span></span>                        | <span data-ttu-id="790a9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="790a9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="790a9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="790a9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="790a9-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="790a9-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="790a9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="790a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="790a9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790a9-117">Not supported.</span></span> |
|<span data-ttu-id="790a9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="790a9-118">Application</span></span>                            | <span data-ttu-id="790a9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790a9-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="790a9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="790a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="790a9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="790a9-121">Request headers</span></span>
| <span data-ttu-id="790a9-122">Name</span><span class="sxs-lookup"><span data-stu-id="790a9-122">Name</span></span>         | <span data-ttu-id="790a9-123">Typ</span><span class="sxs-lookup"><span data-stu-id="790a9-123">Type</span></span>        | <span data-ttu-id="790a9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790a9-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="790a9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="790a9-125">Authorization</span></span> | <span data-ttu-id="790a9-126">string</span><span class="sxs-lookup"><span data-stu-id="790a9-126">string</span></span> | <span data-ttu-id="790a9-127">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="790a9-127">Bearer \{token\}.</span></span> <span data-ttu-id="790a9-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="790a9-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="790a9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="790a9-129">Request body</span></span>
<span data-ttu-id="790a9-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Parameter eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="790a9-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="790a9-131">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="790a9-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="790a9-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="790a9-132">Property</span></span>     | <span data-ttu-id="790a9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="790a9-133">Type</span></span>        | <span data-ttu-id="790a9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790a9-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="790a9-135">Der Name des Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="790a9-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="790a9-136">Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="790a9-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="790a9-137">Dies muss ein Datum in der Zukunft sein.</span><span class="sxs-lookup"><span data-stu-id="790a9-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="790a9-138">Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden.</span><span class="sxs-lookup"><span data-stu-id="790a9-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="790a9-139">Dies muss mindestens einen Tag später als das Startdatum sein.</span><span class="sxs-lookup"><span data-stu-id="790a9-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="790a9-140">Die Beschreibung für die Bearbeiter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="790a9-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="790a9-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="790a9-141">Response</span></span>
<span data-ttu-id="790a9-142">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `204, Accepted` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="790a9-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="790a9-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="790a9-143">Example</span></span>

<span data-ttu-id="790a9-144">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="790a9-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="790a9-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="790a9-145">Request</span></span>
<span data-ttu-id="790a9-146">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der neuen Eigenschaften des [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="790a9-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="790a9-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="790a9-147">Response</span></span>
><span data-ttu-id="790a9-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="790a9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
