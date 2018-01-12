# <a name="get-user-mailbox-settings"></a><span data-ttu-id="b8207-101">Postfacheinstellungen des Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="b8207-101">Get user mailbox settings</span></span>

<span data-ttu-id="b8207-p101">Rufen Sie die [mailboxSettings](../resources/mailboxsettings.md) des Benutzers ab. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema (Sprache und Land/Region) und Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="b8207-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="b8207-104">Sie können alle Postfacheinstellungen anzeigen oder bestimmte Einstellungen abrufen.</span><span class="sxs-lookup"><span data-stu-id="b8207-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="b8207-105">Zeitzone ist eine bevorzugte Einstellung, die ein Benutzer für das Benutzerpostfach einrichten kann.</span><span class="sxs-lookup"><span data-stu-id="b8207-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="b8207-106">Gültige Zeitzonenformate sind das Windows-Zeitzonenformat und das [IANA-Zeitzonenformat (Internet Assigned Numbers Authority)]((http://www.iana.org/time-zones)) (auch als Olson-Zeitzone bezeichnet).</span><span class="sxs-lookup"><span data-stu-id="b8207-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span> <span data-ttu-id="b8207-107">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="b8207-107">The Windows format is the default.</span></span> 

<span data-ttu-id="b8207-108">Wenn Sie die bevorzugte Zeitzone eines Benutzers abrufen, wird die Zeitzone in dem eingerichteten Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8207-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="b8207-109">Wenn Sie diese Zeitzone in einem bestimmten Format (Windows oder IANA) abrufen möchten, können Sie zunächst [die bevorzugte Zeitzone in das entsprechende Format als Postfacheinstellung ändern](user_update_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b8207-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="b8207-110">Anschließend können Sie die Zeitzone in diesem Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="b8207-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="b8207-111">Alternativ können Sie die Formatkonvertierung separat in Ihrer App verwalten.</span><span class="sxs-lookup"><span data-stu-id="b8207-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8207-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8207-112">Permissions</span></span>
<span data-ttu-id="b8207-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8207-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8207-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8207-115">Permission type</span></span>      | <span data-ttu-id="b8207-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8207-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8207-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8207-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b8207-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8207-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8207-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8207-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8207-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8207-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8207-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8207-121">Application</span></span> | <span data-ttu-id="b8207-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8207-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8207-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8207-123">HTTP request</span></span>
<span data-ttu-id="b8207-124">Verwenden Sie die folgende Anforderung, um alle Postfacheinstellungen einschließlich Einstellungen für automatische Antworten abzurufen:</span><span class="sxs-lookup"><span data-stu-id="b8207-124">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="b8207-125">Verwenden Sie die folgende Anforderung, um bestimmte Einstellungen abzurufen, z. B. Einstellungen für automatische Antworten, Gebietsschema oder Zeitzone:</span><span class="sxs-lookup"><span data-stu-id="b8207-125">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8207-126">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8207-126">Optional query parameters</span></span>
<span data-ttu-id="b8207-127">Diese Methode unterstützt die [OData-Abfrageparameter]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8207-127">This method supports the [OData Query Parameters]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b8207-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8207-128">Request headers</span></span>
| <span data-ttu-id="b8207-129">Name</span><span class="sxs-lookup"><span data-stu-id="b8207-129">Name</span></span>       | <span data-ttu-id="b8207-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b8207-130">Type</span></span> | <span data-ttu-id="b8207-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8207-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8207-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8207-132">Authorization</span></span>  | <span data-ttu-id="b8207-133">string</span><span class="sxs-lookup"><span data-stu-id="b8207-133">string</span></span>  | <span data-ttu-id="b8207-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8207-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8207-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8207-136">Request body</span></span>
<span data-ttu-id="b8207-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8207-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8207-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8207-138">Response</span></span>

<span data-ttu-id="b8207-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eines der folgenden angeforderten Objekte im Antworttext zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="b8207-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="b8207-140">[mailboxSettings](../resources/mailboxsettings.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b8207-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="b8207-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b8207-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="b8207-142">[localeInfo](../resources/localeinfo.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b8207-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="b8207-143">Zeichenfolge (für **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="b8207-143">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="b8207-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8207-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b8207-145">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="b8207-145">Request 1</span></span>
<span data-ttu-id="b8207-146">Im ersten Beispiel werden alle Postfacheinstellungen des Postfachs des angemeldeten Benutzers abgerufen, welche die Einstellungen für automatische Antworten, Zeitzone und Spracheinstellungen umfassen.</span><span class="sxs-lookup"><span data-stu-id="b8207-146">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="b8207-147">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="b8207-147">Response 1</span></span>
<span data-ttu-id="b8207-p106">Die Antwort beinhaltet alle Postfacheinstellungen. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8207-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="b8207-151">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="b8207-151">Request 2</span></span>
<span data-ttu-id="b8207-152">Im zweiten Beispiel werden die Einstellungen für automatische Antworten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b8207-152">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="b8207-153">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="b8207-153">Response 2</span></span>
<span data-ttu-id="b8207-p107">Die Antwort enthält nur die Einstellungen für automatische Antworten. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8207-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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