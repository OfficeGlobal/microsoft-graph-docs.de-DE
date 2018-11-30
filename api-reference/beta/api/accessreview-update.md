---
title: AccessReview aktualisieren
description: In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um eine oder mehrere Eigenschaften ändern.
ms.openlocfilehash: 8913377db8acea17023605f85d01c8c9ecea419b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059363"
---
# <a name="update-accessreview"></a><span data-ttu-id="9a762-103">AccessReview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9a762-103">Update accessReview</span></span>

> <span data-ttu-id="9a762-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9a762-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a762-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a762-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a762-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um eine oder mehrere Eigenschaften ändern.</span><span class="sxs-lookup"><span data-stu-id="9a762-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="9a762-107">Diese API ist nicht so ändern Sie die Bearbeiter oder Entscheidungen einer Überprüfung vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="9a762-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="9a762-108">Um die Bearbeiter ändern möchten, verwenden Sie die [AddReviewer](accessreview-addreviewer.md) oder [RemoveReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="9a762-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="9a762-109">Beenden einer bereits gestartet einmalige Überprüfung oder eine Instanz bereits gestartet eine periodische Überprüfung, frühzeitig und [Beenden](accessreview-stop.md) API verwenden, und um die Entscheidungen auf Ziel Zugriffsrechte Gruppe oder app anzuwenden verwenden Sie die [anwenden](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="9a762-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API, and to apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="9a762-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a762-110">Permissions</span></span>
<span data-ttu-id="9a762-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a762-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a762-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a762-113">Permission type</span></span>                        | <span data-ttu-id="9a762-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a762-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a762-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a762-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a762-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a762-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9a762-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a762-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a762-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a762-118">Not supported.</span></span> |
|<span data-ttu-id="9a762-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a762-119">Application</span></span>                            | <span data-ttu-id="9a762-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a762-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a762-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a762-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="9a762-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a762-122">Request headers</span></span>
| <span data-ttu-id="9a762-123">Name</span><span class="sxs-lookup"><span data-stu-id="9a762-123">Name</span></span>         | <span data-ttu-id="9a762-124">Typ</span><span class="sxs-lookup"><span data-stu-id="9a762-124">Type</span></span>        | <span data-ttu-id="9a762-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a762-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9a762-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a762-126">Authorization</span></span> | <span data-ttu-id="9a762-127">string</span><span class="sxs-lookup"><span data-stu-id="9a762-127">string</span></span> | <span data-ttu-id="9a762-128">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="9a762-128">Bearer \{token\}.</span></span> <span data-ttu-id="9a762-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a762-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a762-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a762-130">Request body</span></span>
<span data-ttu-id="9a762-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ein Parameter eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a762-131">In the request body, supply a JSON representation of a parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="9a762-132">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="9a762-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="9a762-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a762-133">Property</span></span>     | <span data-ttu-id="9a762-134">Typ</span><span class="sxs-lookup"><span data-stu-id="9a762-134">Type</span></span>        | <span data-ttu-id="9a762-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a762-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="9a762-136">Der Name des Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="9a762-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="9a762-137">Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9a762-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="9a762-138">Dies muss ein Datum in der Zukunft sein.</span><span class="sxs-lookup"><span data-stu-id="9a762-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="9a762-139">Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden.</span><span class="sxs-lookup"><span data-stu-id="9a762-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="9a762-140">Dies muss mindestens einen Tag später als das Startdatum sein.</span><span class="sxs-lookup"><span data-stu-id="9a762-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="9a762-141">Die Beschreibung für die Bearbeiter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9a762-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="9a762-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a762-142">Response</span></span>
<span data-ttu-id="9a762-143">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `204, Accepted` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9a762-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a762-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a762-144">Example</span></span>

<span data-ttu-id="9a762-145">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9a762-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="9a762-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a762-146">Request</span></span>
<span data-ttu-id="9a762-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der neuen Eigenschaften des [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a762-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="9a762-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a762-148">Response</span></span>
><span data-ttu-id="9a762-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9a762-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
