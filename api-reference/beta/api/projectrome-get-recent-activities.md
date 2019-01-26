---
title: Abrufen aktueller Benutzeraktivitäten
description: " API. Der Dienst für die aktuelle HistoryItems Abfragen, und ziehen Sie die zugehörigen Aktivitäten. Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert. Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden. Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: f19dc8eea40d61afba8e34891431a73f565d6ec3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573165"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="0011f-109">Abrufen aktueller Benutzeraktivitäten</span><span class="sxs-lookup"><span data-stu-id="0011f-109">Get recent user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0011f-110">Rufen Sie aktuelle Aktivitäten für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="0011f-110">Get recent activities for a given user.</span></span> <span data-ttu-id="0011f-111">Diese OData-Funktion verfügt über einige Standardverhalten enthalten, sodass sie wie eine API "zuletzt verwendet" ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="0011f-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="0011f-112">Der Dienst für die aktuelle [HistoryItems](../resources/projectrome-historyitem.md)Abfragen, und ziehen Sie die zugehörigen Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="0011f-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="0011f-113">Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert.</span><span class="sxs-lookup"><span data-stu-id="0011f-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="0011f-114">Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden.</span><span class="sxs-lookup"><span data-stu-id="0011f-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="0011f-115">Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0011f-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="0011f-116">Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="0011f-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="0011f-117">Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="0011f-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="0011f-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0011f-118">Permissions</span></span>

<span data-ttu-id="0011f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0011f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0011f-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0011f-121">Permission type</span></span>      | <span data-ttu-id="0011f-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0011f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0011f-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0011f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0011f-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0011f-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0011f-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0011f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0011f-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0011f-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0011f-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0011f-127">Application</span></span> | <span data-ttu-id="0011f-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0011f-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0011f-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0011f-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0011f-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0011f-130">Optional query parameters</span></span>

<span data-ttu-id="0011f-131">Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="0011f-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="0011f-132">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="0011f-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="0011f-133">$ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="0011f-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="0011f-134">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="0011f-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="0011f-135">$filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten** oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="0011f-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="0011f-136">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung.</span><span class="sxs-lookup"><span data-stu-id="0011f-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="0011f-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0011f-137">Request headers</span></span>

|<span data-ttu-id="0011f-138">Name</span><span class="sxs-lookup"><span data-stu-id="0011f-138">Name</span></span> | <span data-ttu-id="0011f-139">Typ</span><span class="sxs-lookup"><span data-stu-id="0011f-139">Type</span></span> | <span data-ttu-id="0011f-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0011f-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0011f-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="0011f-141">Authorization</span></span> | <span data-ttu-id="0011f-142">string</span><span class="sxs-lookup"><span data-stu-id="0011f-142">string</span></span> | <span data-ttu-id="0011f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0011f-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0011f-145">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0011f-145">Request body</span></span>

<span data-ttu-id="0011f-146">Geben Sie einen Anforderungstext nicht.</span><span class="sxs-lookup"><span data-stu-id="0011f-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0011f-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0011f-147">Response</span></span>

<span data-ttu-id="0011f-148">Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit den aktuellsten Aktivitäten des Benutzers, für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="0011f-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="0011f-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0011f-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0011f-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0011f-150">Request</span></span>

<span data-ttu-id="0011f-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0011f-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="0011f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="0011f-152">Response</span></span>

<span data-ttu-id="0011f-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0011f-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "microsoft.graph.activity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-recent-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
