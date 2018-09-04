# <a name="get-user-mailbox-settings"></a><span data-ttu-id="9ce90-101">Postfacheinstellungen des Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="9ce90-101">Get user mailbox settings</span></span>

<span data-ttu-id="9ce90-p101">Rufen Sie die [mailboxSettings](../resources/mailboxsettings.md) des Benutzers ab. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema (Sprache und Land/Region), Zeitzone und die Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="9ce90-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone, and working hours.</span></span>

<span data-ttu-id="9ce90-104">Sie können alle Postfacheinstellungen anzeigen oder bestimmte Einstellungen abrufen.</span><span class="sxs-lookup"><span data-stu-id="9ce90-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="9ce90-105">Zeitzone ist eine bevorzugte Einstellung, die ein Benutzer für das Benutzerpostfach einrichten kann.</span><span class="sxs-lookup"><span data-stu-id="9ce90-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="9ce90-106">Gültige Zeitzonenformate sind das Windows-Zeitzonenformat und das [IANA-Zeitzonenformat (Internet Assigned Numbers Authority)](http://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet).</span><span class="sxs-lookup"><span data-stu-id="9ce90-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="9ce90-107">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="9ce90-107">The Windows format is the default.</span></span> 

<span data-ttu-id="9ce90-108">Wenn Sie die bevorzugte Zeitzone eines Benutzers abrufen, wird die Zeitzone in dem eingerichteten Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce90-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="9ce90-109">Wenn Sie diese Zeitzone in einem bestimmten Format (Windows oder IANA) abrufen möchten, können Sie zunächst [die bevorzugte Zeitzone in das entsprechende Format als Postfacheinstellung ändern](user_update_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="9ce90-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="9ce90-110">Anschließend können Sie die Zeitzone in diesem Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="9ce90-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="9ce90-111">Alternativ können Sie die Formatkonvertierung separat in Ihrer App verwalten.</span><span class="sxs-lookup"><span data-stu-id="9ce90-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce90-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ce90-112">Permissions</span></span>
<span data-ttu-id="9ce90-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ce90-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ce90-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ce90-115">Permission type</span></span>      | <span data-ttu-id="9ce90-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ce90-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce90-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ce90-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9ce90-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ce90-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9ce90-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ce90-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ce90-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ce90-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9ce90-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ce90-121">Application</span></span> | <span data-ttu-id="9ce90-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ce90-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ce90-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce90-123">HTTP request</span></span>
<span data-ttu-id="9ce90-124">So rufen Sie alle Postfacheinstellungen für einen Benutzer ab: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9ce90-124">To get all mailbox settings for a user:<!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="9ce90-125">Verwenden Sie die folgende Anforderung, um bestimmte Einstellungen abzurufen, z. B. Einstellungen für automatische Antworten, Gebietsschema, Zeitzone oder Geschäftszeiten: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9ce90-125">To get specific settings - for example, only the automatic replies settings, locale, time zone, or working hours:<!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ce90-126">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ce90-126">Optional query parameters</span></span>
<span data-ttu-id="9ce90-127">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ce90-127">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9ce90-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ce90-128">Request headers</span></span>
| <span data-ttu-id="9ce90-129">Name</span><span class="sxs-lookup"><span data-stu-id="9ce90-129">Name</span></span>       | <span data-ttu-id="9ce90-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9ce90-130">Type</span></span> | <span data-ttu-id="9ce90-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ce90-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9ce90-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9ce90-132">Authorization</span></span>  | <span data-ttu-id="9ce90-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce90-133">string</span></span>  | <span data-ttu-id="9ce90-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ce90-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ce90-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ce90-136">Request body</span></span>
<span data-ttu-id="9ce90-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9ce90-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ce90-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce90-138">Response</span></span>

<span data-ttu-id="9ce90-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eines der folgenden angeforderten Objekte im Antworttext zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="9ce90-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="9ce90-140">[mailboxSettings](../resources/mailboxsettings.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="9ce90-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="9ce90-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="9ce90-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="9ce90-142">[localeInfo](../resources/localeinfo.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="9ce90-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="9ce90-143">Zeichenfolge (für **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="9ce90-143">string (for **timeZone**)</span></span>
- [<span data-ttu-id="9ce90-144">workingHours</span><span class="sxs-lookup"><span data-stu-id="9ce90-144">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="9ce90-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ce90-145">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9ce90-146">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9ce90-146">Request 1</span></span>
<span data-ttu-id="9ce90-147">Im ersten Beispiel werden alle Postfacheinstellungen des Postfachs des angemeldeten Benutzers abgerufen, die Einstellungen für Zeitzone, automatische Antworten, Gebietsschema (Sprache und Land/Region) sowie Geschäftszeiten umfassen.</span><span class="sxs-lookup"><span data-stu-id="9ce90-147">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="9ce90-148">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9ce90-148">Response 1</span></span>
<span data-ttu-id="9ce90-p106">Die Antwort beinhaltet alle Postfacheinstellungen. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce90-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.000",
        "endTime":"17:00:00.000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="9ce90-152">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9ce90-152">Request 2</span></span>
<span data-ttu-id="9ce90-153">Im zweiten Beispiel werden die Einstellungen für automatische Antworten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="9ce90-153">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="9ce90-154">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9ce90-154">Response 2</span></span>
<span data-ttu-id="9ce90-p107">Die Antwort enthält nur die Einstellungen für automatische Antworten. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce90-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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


##### <a name="request-3"></a><span data-ttu-id="9ce90-158">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="9ce90-158">Request 3</span></span>
<span data-ttu-id="9ce90-159">Im dritten Beispiel werden die Einstellungen für die Geschäftszeiten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="9ce90-159">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="9ce90-160">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="9ce90-160">Response 3</span></span>
<span data-ttu-id="9ce90-161">Die Antwort enthält nur die Einstellungen für Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="9ce90-161">The response includes only the working hours settings.</span></span> <span data-ttu-id="9ce90-162">Beachten Sie, dass sich die Geschäftszeiten des Benutzers in einer [benutzerdefinierten Zeitzone](../resources/customtimezone.md) befinden.</span><span class="sxs-lookup"><span data-stu-id="9ce90-162">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="9ce90-163">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9ce90-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ce90-164">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce90-164">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
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