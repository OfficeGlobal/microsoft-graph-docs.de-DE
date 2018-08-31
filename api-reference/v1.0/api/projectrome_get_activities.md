# <a name="get-user-activities"></a><span data-ttu-id="9c825-101">Benutzeraktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="9c825-101">Get user activities</span></span>

<span data-ttu-id="9c825-102">Aktivitäten für einen bestimmten Benutzer abrufen.</span><span class="sxs-lookup"><span data-stu-id="9c825-102">Get activities for a given user.</span></span> <span data-ttu-id="9c825-103">Im Gegensatz zu der **letzten** OData-Funktion werden Aktivitäten ohne Historien zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c825-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="9c825-104">Die Berechtigung UserActivity.ReadWrite.CreatedByApp wendet eine zusätzliche Filterung für die Antwort an, sodass nur von Ihrer Anwendung erstellte Aktivitäten zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9c825-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="9c825-105">Diese serverseitige Filterung kann zu leeren Seiten führen, wenn der Benutzer besonders aktiv ist und andere Anwendungen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="9c825-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="9c825-106">Um die Aktivitäten Ihrer Anwendung zu erhalten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="9c825-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c825-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c825-107">Permissions</span></span>

<span data-ttu-id="9c825-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c825-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c825-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c825-110">Permission type</span></span>      | <span data-ttu-id="9c825-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c825-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c825-112">Delegiert (Arbeits- oder Schulkonto)</span><span class="sxs-lookup"><span data-stu-id="9c825-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c825-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9c825-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9c825-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c825-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c825-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9c825-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9c825-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c825-116">Application</span></span> | <span data-ttu-id="9c825-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c825-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c825-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c825-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c825-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9c825-119">Optional query parameters</span></span>

<span data-ttu-id="9c825-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c825-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="9c825-121">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="9c825-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="9c825-122">$expand Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="9c825-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="9c825-123">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="9c825-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="9c825-124">$filter auf die **LastModifiedDateTime** -Eigenschaft für Aktivitäten oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="9c825-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="9c825-125">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung:</span><span class="sxs-lookup"><span data-stu-id="9c825-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="9c825-126">Anfrage Kopfzeilen</span><span class="sxs-lookup"><span data-stu-id="9c825-126">Request headers</span></span>

|<span data-ttu-id="9c825-127">Name</span><span class="sxs-lookup"><span data-stu-id="9c825-127">Name</span></span> | <span data-ttu-id="9c825-128">Typ</span><span class="sxs-lookup"><span data-stu-id="9c825-128">Type</span></span> | <span data-ttu-id="9c825-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c825-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="9c825-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9c825-130">Authorization</span></span> | <span data-ttu-id="9c825-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c825-131">string</span></span> | <span data-ttu-id="9c825-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c825-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c825-134">Anfragetext</span><span class="sxs-lookup"><span data-stu-id="9c825-134">Request body</span></span>

<span data-ttu-id="9c825-135">Kein Anfragetext.</span><span class="sxs-lookup"><span data-stu-id="9c825-135">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="9c825-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c825-136">Response</span></span>

<span data-ttu-id="9c825-137">Wenn der Vorgang erfolgreich war, gibt diese Methode den `200 OK` Antwortcode mit den Benutzeraktivitäten für ihre Anwendung aus.</span><span class="sxs-lookup"><span data-stu-id="9c825-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="9c825-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c825-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9c825-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c825-139">Request</span></span>

<span data-ttu-id="9c825-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c825-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="9c825-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c825-141">Response</span></span>

<span data-ttu-id="9c825-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c825-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
