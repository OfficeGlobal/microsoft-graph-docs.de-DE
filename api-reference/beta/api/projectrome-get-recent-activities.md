---
title: Abrufen aktueller Benutzeraktivitäten
description: " API. Der Dienst für die aktuelle HistoryItems Abfragen, und ziehen Sie die zugehörigen Aktivitäten. Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert. Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden. Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung."
ms.openlocfilehash: 7dbd51e416d62016add020b784b0f7d0ace473cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066109"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="78a87-109">Abrufen aktueller Benutzeraktivitäten</span><span class="sxs-lookup"><span data-stu-id="78a87-109">Get recent user activities</span></span>

> <span data-ttu-id="78a87-110">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78a87-110">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78a87-111">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78a87-111">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78a87-112">Rufen Sie aktuelle Aktivitäten für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="78a87-112">Get recent activities for a given user.</span></span> <span data-ttu-id="78a87-113">Diese OData-Funktion verfügt über einige Standardverhalten enthalten, sodass sie wie eine API "zuletzt verwendet" ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="78a87-113">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="78a87-114">Der Dienst für die aktuelle [HistoryItems](../resources/projectrome-historyitem.md)Abfragen, und ziehen Sie die zugehörigen Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="78a87-114">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="78a87-115">Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert.</span><span class="sxs-lookup"><span data-stu-id="78a87-115">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="78a87-116">Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden.</span><span class="sxs-lookup"><span data-stu-id="78a87-116">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="78a87-117">Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="78a87-117">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="78a87-118">Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="78a87-118">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="78a87-119">Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="78a87-119">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="78a87-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="78a87-120">Permissions</span></span>

<span data-ttu-id="78a87-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78a87-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78a87-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78a87-123">Permission type</span></span>      | <span data-ttu-id="78a87-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78a87-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78a87-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78a87-125">Delegated (work or school account)</span></span> | <span data-ttu-id="78a87-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="78a87-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="78a87-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78a87-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78a87-128">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="78a87-128">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="78a87-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78a87-129">Application</span></span> | <span data-ttu-id="78a87-130">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78a87-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78a87-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78a87-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78a87-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="78a87-132">Optional query parameters</span></span>

<span data-ttu-id="78a87-133">Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="78a87-133">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="78a87-134">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="78a87-134">The following query parameters are supported:</span></span>

- <span data-ttu-id="78a87-135">$ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="78a87-135">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="78a87-136">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="78a87-136">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="78a87-137">$filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten** oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="78a87-137">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="78a87-138">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung.</span><span class="sxs-lookup"><span data-stu-id="78a87-138">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="78a87-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78a87-139">Request headers</span></span>

|<span data-ttu-id="78a87-140">Name</span><span class="sxs-lookup"><span data-stu-id="78a87-140">Name</span></span> | <span data-ttu-id="78a87-141">Typ</span><span class="sxs-lookup"><span data-stu-id="78a87-141">Type</span></span> | <span data-ttu-id="78a87-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78a87-142">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="78a87-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="78a87-143">Authorization</span></span> | <span data-ttu-id="78a87-144">string</span><span class="sxs-lookup"><span data-stu-id="78a87-144">string</span></span> | <span data-ttu-id="78a87-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="78a87-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78a87-147">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78a87-147">Request body</span></span>

<span data-ttu-id="78a87-148">Geben Sie einen Anforderungstext nicht.</span><span class="sxs-lookup"><span data-stu-id="78a87-148">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="78a87-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="78a87-149">Response</span></span>

<span data-ttu-id="78a87-150">Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit den aktuellsten Aktivitäten des Benutzers, für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="78a87-150">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="78a87-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78a87-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78a87-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78a87-152">Request</span></span>

<span data-ttu-id="78a87-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78a87-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="78a87-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="78a87-154">Response</span></span>

<span data-ttu-id="78a87-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="78a87-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
