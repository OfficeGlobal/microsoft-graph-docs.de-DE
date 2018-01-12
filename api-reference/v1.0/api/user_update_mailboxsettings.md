# <a name="update-user-mailbox-settings"></a><span data-ttu-id="87b32-101">Postfacheinstellungen des Benutzers aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87b32-101">Update user mailbox settings</span></span>

<span data-ttu-id="87b32-p101">Dient zum Aktualisieren von Einstellungen für das Postfach des Benutzers. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema oder Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="87b32-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="87b32-104">Diese Einstellungen können Sie im Rahmen des [mailboxSettings](../resources/mailboxsettings.md)-Elements aktivieren, konfigurieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="87b32-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="87b32-105">**Hinweis:** Sie können keine Postfacheinstellungen erstellen oder löschen.</span><span class="sxs-lookup"><span data-stu-id="87b32-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="87b32-106">Wenn Sie die bevorzugte Zeitzone für einen Benutzer aktualisieren, können Sie diese im Windows- oder im [IANA-Format]((http://www.iana.org/time-zones)) (auch als Olson-Zeitzone bezeichnet) angeben.</span><span class="sxs-lookup"><span data-stu-id="87b32-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="87b32-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87b32-107">Permissions</span></span>
<span data-ttu-id="87b32-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87b32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87b32-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87b32-110">Permission type</span></span>      | <span data-ttu-id="87b32-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87b32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87b32-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87b32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87b32-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87b32-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="87b32-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87b32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87b32-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87b32-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="87b32-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87b32-116">Application</span></span> | <span data-ttu-id="87b32-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87b32-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="87b32-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87b32-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87b32-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87b32-119">Optional query parameters</span></span>
<span data-ttu-id="87b32-120">Diese Methode unterstützt die [OData-Abfrageparameter]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87b32-120">This method supports the [OData Query Parameters]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87b32-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87b32-121">Request headers</span></span>
| <span data-ttu-id="87b32-122">Name</span><span class="sxs-lookup"><span data-stu-id="87b32-122">Name</span></span>       | <span data-ttu-id="87b32-123">Typ</span><span class="sxs-lookup"><span data-stu-id="87b32-123">Type</span></span> | <span data-ttu-id="87b32-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87b32-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87b32-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87b32-125">Authorization</span></span>  | <span data-ttu-id="87b32-126">string</span><span class="sxs-lookup"><span data-stu-id="87b32-126">string</span></span>  | <span data-ttu-id="87b32-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87b32-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87b32-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87b32-129">Request body</span></span>
<span data-ttu-id="87b32-p104">Geben Sie im Anforderungstext die Werte für die relevanten Eigenschaften an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Im Folgenden werden die beschreibbaren/aktualisierbaren Eigenschaften aufgelistet:</span><span class="sxs-lookup"><span data-stu-id="87b32-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="87b32-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87b32-134">Property</span></span>     | <span data-ttu-id="87b32-135">Typ</span><span class="sxs-lookup"><span data-stu-id="87b32-135">Type</span></span>   |<span data-ttu-id="87b32-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87b32-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87b32-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="87b32-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="87b32-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="87b32-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="87b32-139">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="87b32-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="87b32-140">language</span><span class="sxs-lookup"><span data-stu-id="87b32-140">language</span></span>|[<span data-ttu-id="87b32-141">localeInfo</span><span class="sxs-lookup"><span data-stu-id="87b32-141">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="87b32-142">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="87b32-142">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="87b32-143">timeZone</span><span class="sxs-lookup"><span data-stu-id="87b32-143">timeZone</span></span>|<span data-ttu-id="87b32-144">string</span><span class="sxs-lookup"><span data-stu-id="87b32-144">string</span></span>|<span data-ttu-id="87b32-145">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="87b32-145">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="87b32-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="87b32-146">Response</span></span>

<span data-ttu-id="87b32-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [mailboxSettings](../resources/mailboxSettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87b32-147">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87b32-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87b32-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87b32-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87b32-149">Request</span></span>
<span data-ttu-id="87b32-150">Im folgende Beispiel werden automatische Antworten für einen bestimmten Datumsbereich durch Festlegen der folgenden Eigenschaften der **automaticRepliesSetting**-Eigenschaft aktiviert: **status**, **scheduledStartDateTime** und **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="87b32-150">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/api/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response"></a><span data-ttu-id="87b32-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="87b32-151">Response</span></span>
<span data-ttu-id="87b32-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87b32-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "none",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->