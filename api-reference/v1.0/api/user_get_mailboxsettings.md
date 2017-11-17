# <a name="get-user-mailbox-settings"></a><span data-ttu-id="1f24d-101">Postfacheinstellungen des Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="1f24d-101">Get user mailbox settings</span></span>

<span data-ttu-id="1f24d-p101">Rufen Sie die [mailboxSettings](../resources/mailboxsettings.md) des Benutzers ab. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema (Sprache und Land/Region) und Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="1f24d-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="1f24d-104">Sie können alle Postfacheinstellungen anzeigen oder bestimmte Einstellungen abrufen.</span><span class="sxs-lookup"><span data-stu-id="1f24d-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f24d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f24d-105">Permissions</span></span>
<span data-ttu-id="1f24d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f24d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f24d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f24d-108">Permission type</span></span>      | <span data-ttu-id="1f24d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f24d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f24d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f24d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f24d-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f24d-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1f24d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f24d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f24d-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f24d-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1f24d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f24d-114">Application</span></span> | <span data-ttu-id="1f24d-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f24d-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f24d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f24d-116">HTTP request</span></span>
<span data-ttu-id="1f24d-117">Verwenden Sie die folgende Anforderung, um alle Postfacheinstellungen einschließlich Einstellungen für automatische Antworten abzurufen:</span><span class="sxs-lookup"><span data-stu-id="1f24d-117">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="1f24d-118">Verwenden Sie die folgende Anforderung, um bestimmte Einstellungen abzurufen, z. B. Einstellungen für automatische Antworten, Gebietsschema oder Zeitzone:</span><span class="sxs-lookup"><span data-stu-id="1f24d-118">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f24d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f24d-119">Optional query parameters</span></span>
<span data-ttu-id="1f24d-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f24d-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f24d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f24d-121">Request headers</span></span>
| <span data-ttu-id="1f24d-122">Name</span><span class="sxs-lookup"><span data-stu-id="1f24d-122">Name</span></span>       | <span data-ttu-id="1f24d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="1f24d-123">Type</span></span> | <span data-ttu-id="1f24d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f24d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f24d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f24d-125">Authorization</span></span>  | <span data-ttu-id="1f24d-126">string</span><span class="sxs-lookup"><span data-stu-id="1f24d-126">string</span></span>  | <span data-ttu-id="1f24d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f24d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f24d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f24d-129">Request body</span></span>
<span data-ttu-id="1f24d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f24d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f24d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f24d-131">Response</span></span>

<span data-ttu-id="1f24d-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eines der folgenden angeforderten Objekte im Antworttext zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="1f24d-132">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="1f24d-133">[mailboxSettings](../resources/mailboxsettings.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="1f24d-133">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="1f24d-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="1f24d-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="1f24d-135">[localeInfo](../resources/localeinfo.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="1f24d-135">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="1f24d-136">Zeichenfolge (für **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="1f24d-136">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="1f24d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f24d-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1f24d-138">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="1f24d-138">Request 1</span></span>
<span data-ttu-id="1f24d-139">Im ersten Beispiel werden alle Postfacheinstellungen des Postfachs des angemeldeten Benutzers abgerufen, welche die Einstellungen für automatische Antworten, Zeitzone und Spracheinstellungen umfassen.</span><span class="sxs-lookup"><span data-stu-id="1f24d-139">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="1f24d-140">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="1f24d-140">Response 1</span></span>
<span data-ttu-id="1f24d-p104">Die Antwort beinhaltet alle Postfacheinstellungen. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f24d-p104">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="1f24d-144">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="1f24d-144">Request 2</span></span>
<span data-ttu-id="1f24d-145">Im zweiten Beispiel werden die Einstellungen für automatische Antworten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="1f24d-145">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="1f24d-146">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="1f24d-146">Response 2</span></span>
<span data-ttu-id="1f24d-p105">Die Antwort enthält nur die Einstellungen für automatische Antworten. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f24d-p105">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->