---
title: AccessReview aktualisieren
description: In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um eine oder mehrere Eigenschaften ändern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e74daa092c6f18c845c7f0c468af90385b899b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016751"
---
# <a name="update-accessreview"></a><span data-ttu-id="79503-103">AccessReview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="79503-103">Update accessReview</span></span>

> <span data-ttu-id="79503-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79503-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79503-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79503-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79503-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um eine oder mehrere Eigenschaften ändern.</span><span class="sxs-lookup"><span data-stu-id="79503-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="79503-107">Diese API ist nicht so ändern Sie die Bearbeiter oder Entscheidungen einer Überprüfung vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="79503-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="79503-108">Um die Bearbeiter ändern möchten, verwenden Sie die [AddReviewer](accessreview-addreviewer.md) oder [RemoveReviewer](accessreview-removereviewer.md) APIs.</span><span class="sxs-lookup"><span data-stu-id="79503-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="79503-109">Verwenden Sie eine einmalige Überprüfung bei bereits gestartet, oder eine Instanz bereits gestartet periodische Wiederholung frühzeitig und, um beenden [Beenden](accessreview-stop.md) API.</span><span class="sxs-lookup"><span data-stu-id="79503-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="79503-110">Um die Entscheidungen über die Ziel-Gruppe oder app Zugriffsrechte anwenden möchten, verwenden Sie die [anwenden](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="79503-110">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="79503-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79503-111">Permissions</span></span>
<span data-ttu-id="79503-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79503-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79503-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79503-114">Permission type</span></span>                        | <span data-ttu-id="79503-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79503-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="79503-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79503-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="79503-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79503-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="79503-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79503-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79503-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79503-119">Not supported.</span></span> |
|<span data-ttu-id="79503-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79503-120">Application</span></span>                            | <span data-ttu-id="79503-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79503-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79503-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79503-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="79503-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79503-123">Request headers</span></span>
| <span data-ttu-id="79503-124">Name</span><span class="sxs-lookup"><span data-stu-id="79503-124">Name</span></span>         | <span data-ttu-id="79503-125">Typ</span><span class="sxs-lookup"><span data-stu-id="79503-125">Type</span></span>        | <span data-ttu-id="79503-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79503-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="79503-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="79503-127">Authorization</span></span> | <span data-ttu-id="79503-128">String</span><span class="sxs-lookup"><span data-stu-id="79503-128">string</span></span> | <span data-ttu-id="79503-129">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="79503-129">Bearer \{token\}.</span></span> <span data-ttu-id="79503-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79503-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79503-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79503-131">Request body</span></span>
<span data-ttu-id="79503-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Parameter eines [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="79503-132">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="79503-133">In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.</span><span class="sxs-lookup"><span data-stu-id="79503-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="79503-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79503-134">Property</span></span>     | <span data-ttu-id="79503-135">Typ</span><span class="sxs-lookup"><span data-stu-id="79503-135">Type</span></span>        | <span data-ttu-id="79503-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79503-136">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="79503-137">Der Name des Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="79503-137">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="79503-138">Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="79503-138">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="79503-139">Dies muss ein Datum in der Zukunft sein.</span><span class="sxs-lookup"><span data-stu-id="79503-139">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="79503-140">Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden.</span><span class="sxs-lookup"><span data-stu-id="79503-140">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="79503-141">Dies muss mindestens einen Tag später als das Startdatum sein.</span><span class="sxs-lookup"><span data-stu-id="79503-141">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="79503-142">Die Beschreibung für die Bearbeiter angezeigt.</span><span class="sxs-lookup"><span data-stu-id="79503-142">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="79503-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="79503-143">Response</span></span>
<span data-ttu-id="79503-144">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `204, Accepted` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="79503-144">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79503-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79503-145">Example</span></span>

<span data-ttu-id="79503-146">Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="79503-146">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="79503-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79503-147">Request</span></span>
<span data-ttu-id="79503-148">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der neuen Eigenschaften des [AccessReview](../resources/accessreview.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="79503-148">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="79503-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="79503-149">Response</span></span>
><span data-ttu-id="79503-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="79503-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
