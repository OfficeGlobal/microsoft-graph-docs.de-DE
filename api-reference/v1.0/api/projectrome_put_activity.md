# <a name="create-or-replace-an-activity"></a><span data-ttu-id="e3b32-101">Aktivität erstellen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="e3b32-101">Create or replace an activity</span></span>

<span data-ttu-id="e3b32-102">Erstellen Sie eine neue oder ersetzen Sie eine vorhandene Benutzeraktivität für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="e3b32-102">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="e3b32-103">Für die Erstellung einer Benutzeraktivität und der zugehörigen **HistoryItems** in einer Anforderung können Sie [deep insert](projectrome_put_activity.md#example-2---deep-insert) verwenden.</span><span class="sxs-lookup"><span data-stu-id="e3b32-103">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome_put_activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b32-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3b32-104">Permissions</span></span>

<span data-ttu-id="e3b32-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3b32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e3b32-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3b32-107">Permission type</span></span>      | <span data-ttu-id="e3b32-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3b32-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3b32-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3b32-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b32-110">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e3b32-110">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e3b32-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3b32-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b32-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e3b32-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e3b32-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3b32-113">Application</span></span> | <span data-ttu-id="e3b32-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3b32-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3b32-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3b32-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="e3b32-116">**Hinweis:** Die appActivityId muss URL-sicher sein (alle Zeichen außer RFC 2396 nicht reservierter Zeichen müssen in ihre hexadezimale Darstellung konvertiert werden), aber die ursprüngliche appActivityId muss nicht URL-sicher sein.</span><span class="sxs-lookup"><span data-stu-id="e3b32-116">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3b32-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3b32-117">Request headers</span></span>

|<span data-ttu-id="e3b32-118">Name</span><span class="sxs-lookup"><span data-stu-id="e3b32-118">Name</span></span> | <span data-ttu-id="e3b32-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e3b32-119">Type</span></span> | <span data-ttu-id="e3b32-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3b32-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e3b32-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e3b32-121">Authorization</span></span> | <span data-ttu-id="e3b32-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3b32-122">string</span></span> | <span data-ttu-id="e3b32-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3b32-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3b32-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3b32-125">Request body</span></span>

<span data-ttu-id="e3b32-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/projectrome_activity.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e3b32-126">In the request body, supply a JSON representation of an [educationUser](../resources/projectrome_activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3b32-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3b32-127">Response</span></span>

<span data-ttu-id="e3b32-128">Wenn der Vorgang erfolgreich war, gibt dieses Verfahren den `201 Created` Antwortcode zurück, wenn die Aktivität erstellt wurde oder `200 OK`, wenn die Aktivität ersetzt wurde.</span><span class="sxs-lookup"><span data-stu-id="e3b32-128">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="e3b32-129">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="e3b32-129">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="e3b32-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3b32-130">Request</span></span>

<span data-ttu-id="e3b32-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3b32-131">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="e3b32-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3b32-132">Response</span></span>

<span data-ttu-id="e3b32-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3b32-133">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "http://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="e3b32-134">Beispiel 2 – Deep insert</span><span class="sxs-lookup"><span data-stu-id="e3b32-134">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="e3b32-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3b32-135">Request</span></span>

<span data-ttu-id="e3b32-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3b32-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
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
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="e3b32-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3b32-137">Response</span></span>

<span data-ttu-id="e3b32-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3b32-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "http://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
