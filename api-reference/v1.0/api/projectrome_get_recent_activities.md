# <a name="get-recent-user-activities"></a><span data-ttu-id="e8697-101">Aktuelle Nutzeraktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="e8697-101">Get recent activities</span></span>

<span data-ttu-id="e8697-102">Letzte Aktivitäten für einen bestimmten Benutzer abrufen.</span><span class="sxs-lookup"><span data-stu-id="e8697-102">Get recent activities for a given user.</span></span> <span data-ttu-id="e8697-103">Diese OData-Funktion verfügt über einige Standardverhalten, sodass sie wie eine "zuletzt verwendet"-API  ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="e8697-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="e8697-104">Der Dienst fragt die aktuellen [HistoryItems](../resources/projectrome_historyitem.md) ab und zieht diese zugehörigen Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="e8697-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="e8697-105">Aktivitäten werden entsprechend der neuesten **lastModified** im **historyItem** sortiert.</span><span class="sxs-lookup"><span data-stu-id="e8697-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="e8697-106">Dies bedeutet, dass Aktivitäten ohne **historyItems** nicht in der Antwort enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="e8697-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="e8697-107">Die Berechtigung UserActivity.ReadWrite.CreatedByApp wendet auch eine zusätzliche Filterung für die Antwort an, sodass nur von Ihrer Anwendung erstellte Aktivitäten zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e8697-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="e8697-108">Diese serverseitige Filterung kann zu leeren Seiten führen, wenn der Benutzer besonders aktiv ist und andere Anwendungen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="e8697-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="e8697-109">Um die Aktivitäten Ihrer Anwendung abzurufen, verwenden Sie die **NextLink**-Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="e8697-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8697-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8697-110">Permissions</span></span>

<span data-ttu-id="e8697-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8697-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8697-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8697-113">Permission type</span></span>      | <span data-ttu-id="e8697-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8697-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8697-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8697-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e8697-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e8697-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e8697-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8697-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8697-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e8697-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e8697-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8697-119">Application</span></span> | <span data-ttu-id="e8697-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8697-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8697-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8697-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8697-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e8697-122">Optional query parameters</span></span>

<span data-ttu-id="e8697-123">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8697-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="e8697-124">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="e8697-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="e8697-125">$expand Sie für die Navigationseigenschaft **historyItems**.</span><span class="sxs-lookup"><span data-stu-id="e8697-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="e8697-126">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="e8697-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="e8697-127">$filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten**  oder ** HistoryItems**, falls erweitert.</span><span class="sxs-lookup"><span data-stu-id="e8697-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="e8697-128">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung.</span><span class="sxs-lookup"><span data-stu-id="e8697-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="e8697-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8697-129">Request headers</span></span>

|<span data-ttu-id="e8697-130">Name</span><span class="sxs-lookup"><span data-stu-id="e8697-130">Name</span></span> | <span data-ttu-id="e8697-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e8697-131">Type</span></span> | <span data-ttu-id="e8697-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8697-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e8697-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e8697-133">Authorization</span></span> | <span data-ttu-id="e8697-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8697-134">string</span></span> | <span data-ttu-id="e8697-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8697-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8697-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8697-137">Request body</span></span>

<span data-ttu-id="e8697-138">Geben Sie keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8697-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8697-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8697-139">Response</span></span>

<span data-ttu-id="e8697-140">Wenn der Vorgang erfolgreich war, gibt diese Methode den `200 OK` Antwortcode mit den neuesten Benutzeraktivitäten für ihre Anwendung aus.</span><span class="sxs-lookup"><span data-stu-id="e8697-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="e8697-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8697-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8697-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8697-142">Request</span></span>

<span data-ttu-id="e8697-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8697-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="e8697-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8697-144">Response</span></span>

<span data-ttu-id="e8697-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8697-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "http://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "http://www.contoso.com/article?id=12345",
        "contentUrl": "http://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "http://schema.org",
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
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
