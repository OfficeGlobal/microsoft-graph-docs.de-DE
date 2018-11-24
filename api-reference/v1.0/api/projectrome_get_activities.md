# <a name="get-user-activities"></a><span data-ttu-id="68efb-101">Die Benutzeraktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="68efb-101">Get user activities</span></span>

<span data-ttu-id="68efb-102">Rufen Sie Aktivitäten für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="68efb-102">Get activities for a given user.</span></span> <span data-ttu-id="68efb-103">Aktivitäten ohne gespeichert werden soll, im Gegensatz zu der **letzte** OData-Funktion zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68efb-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="68efb-104">Die Berechtigung UserActivity.ReadWrite.CreatedByApp gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="68efb-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="68efb-105">Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="68efb-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="68efb-106">Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="68efb-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="68efb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68efb-107">Permissions</span></span>

<span data-ttu-id="68efb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68efb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68efb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68efb-110">Permission type</span></span>      | <span data-ttu-id="68efb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68efb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68efb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68efb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68efb-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="68efb-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="68efb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68efb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68efb-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="68efb-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="68efb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68efb-116">Application</span></span> | <span data-ttu-id="68efb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68efb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68efb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68efb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68efb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68efb-119">Optional query parameters</span></span>

<span data-ttu-id="68efb-120">Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="68efb-120">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="68efb-121">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="68efb-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="68efb-122">$ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="68efb-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="68efb-123">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="68efb-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="68efb-124">$filter auf die **LastModifiedDateTime** -Eigenschaft für Aktivitäten oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="68efb-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="68efb-125">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung:</span><span class="sxs-lookup"><span data-stu-id="68efb-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="68efb-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68efb-126">Request headers</span></span>

|<span data-ttu-id="68efb-127">Name</span><span class="sxs-lookup"><span data-stu-id="68efb-127">Name</span></span> | <span data-ttu-id="68efb-128">Typ</span><span class="sxs-lookup"><span data-stu-id="68efb-128">Type</span></span> | <span data-ttu-id="68efb-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68efb-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="68efb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="68efb-130">Authorization</span></span> | <span data-ttu-id="68efb-131">string</span><span class="sxs-lookup"><span data-stu-id="68efb-131">string</span></span> | <span data-ttu-id="68efb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68efb-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68efb-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68efb-134">Request body</span></span>

<span data-ttu-id="68efb-135">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="68efb-135">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="68efb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="68efb-136">Response</span></span>

<span data-ttu-id="68efb-137">Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit die Aktivitäten des Benutzers für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="68efb-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="68efb-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68efb-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68efb-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68efb-139">Request</span></span>

<span data-ttu-id="68efb-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68efb-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="68efb-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="68efb-141">Response</span></span>

<span data-ttu-id="68efb-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68efb-142">The following is an example of the response.</span></span>

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
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
