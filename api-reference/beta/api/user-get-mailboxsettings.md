---
title: Postfacheinstellungen des Benutzers abrufen
description: 'Abrufen des Benutzers MailboxSettings. Einschließlich der Einstellungen für automatische Antworten (Personen automatisch beim Benachrichtigen '
localization_priority: Normal
ms.openlocfilehash: 2d1e2ce16d82e89e701bbe90386c28b76d1607c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880178"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="b0cd3-104">Postfacheinstellungen des Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="b0cd3-104">Get user mailbox settings</span></span>

> <span data-ttu-id="b0cd3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0cd3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0cd3-107">Abrufen des Benutzers [MailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b0cd3-107">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="b0cd3-108">Einschließlich der Einstellungen für automatische Antworten (benachrichtigen Personen automatisch beim Empfang von e-Mails), Gebietsschema (Sprache und Land/Region), Zeitzone und Arbeitszeiten.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-108">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="b0cd3-109">Sie können alle Postfacheinstellungen anzeigen oder bestimmte Einstellungen abrufen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-109">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="b0cd3-110">Zeitzone ist eine bevorzugte Einstellung, die ein Benutzer für das Benutzerpostfach einrichten kann.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-110">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="b0cd3-111">Der Benutzer wählt ihn aus der [Zeitzonen unterstützt](outlookuser-supportedtimezones.md) , die ein Administrator für Postfachserver des Benutzers eingerichtet hat.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-111">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="b0cd3-112">Der Administrator richtet Zeitzonen in der Windows Zeitzone oder [Zeitzone (IANA = Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone)-Format.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-112">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="b0cd3-113">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-113">The Windows format is the default.</span></span> 

<span data-ttu-id="b0cd3-114">Wenn Sie die bevorzugte Zeitzone eines Benutzers abrufen, wird die Zeitzone in dem eingerichteten Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-114">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="b0cd3-115">Wenn Sie diese Zeitzone in einem bestimmten Format (Windows oder IANA) abrufen möchten, können Sie zunächst [die bevorzugte Zeitzone in das entsprechende Format als Postfacheinstellung ändern](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b0cd3-115">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="b0cd3-116">Anschließend können Sie die Zeitzone in diesem Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-116">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="b0cd3-117">Alternativ können Sie die Formatkonvertierung separat in Ihrer App verwalten.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-117">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0cd3-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b0cd3-118">Permissions</span></span>
<span data-ttu-id="b0cd3-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0cd3-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0cd3-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0cd3-121">Permission type</span></span>      | <span data-ttu-id="b0cd3-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0cd3-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-123">Delegated (work or school account)</span></span> | <span data-ttu-id="b0cd3-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0cd3-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b0cd3-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0cd3-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0cd3-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b0cd3-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0cd3-127">Application</span></span> | <span data-ttu-id="b0cd3-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0cd3-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0cd3-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0cd3-129">HTTP request</span></span>
<span data-ttu-id="b0cd3-130">Um die postfacheinstellungen für einen Benutzer abzurufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="b0cd3-130">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="b0cd3-131">Bestimmte Einstellungen - Einstellungen für automatische Antworten, Gebietsschema, Zeitzone oder Arbeitszeiten abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="b0cd3-131">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="b0cd3-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b0cd3-132">Optional query parameters</span></span>
<span data-ttu-id="b0cd3-133">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0cd3-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0cd3-134">Request headers</span></span>
| <span data-ttu-id="b0cd3-135">Name</span><span class="sxs-lookup"><span data-stu-id="b0cd3-135">Name</span></span>       | <span data-ttu-id="b0cd3-136">Typ</span><span class="sxs-lookup"><span data-stu-id="b0cd3-136">Type</span></span> | <span data-ttu-id="b0cd3-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0cd3-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b0cd3-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0cd3-138">Authorization</span></span>  | <span data-ttu-id="b0cd3-139">string</span><span class="sxs-lookup"><span data-stu-id="b0cd3-139">string</span></span>  | <span data-ttu-id="b0cd3-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0cd3-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0cd3-142">Request body</span></span>
<span data-ttu-id="b0cd3-143">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0cd3-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0cd3-144">Response</span></span>

<span data-ttu-id="b0cd3-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eines der folgenden angeforderten Objekte im Antworttext zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="b0cd3-145">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="b0cd3-146">[mailboxSettings](../resources/mailboxsettings.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b0cd3-146">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="b0cd3-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b0cd3-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="b0cd3-148">[localeInfo](../resources/localeinfo.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="b0cd3-148">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="b0cd3-149">Zeichenfolge (für **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-149">string (for **timeZone**)</span></span>
- [<span data-ttu-id="b0cd3-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="b0cd3-150">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="b0cd3-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0cd3-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b0cd3-152">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="b0cd3-152">Request 1</span></span>
<span data-ttu-id="b0cd3-153">Im ersten Beispiel werden alle Postfacheinstellungen des Postfachs des angemeldeten Benutzers abgerufen, die Einstellungen für Zeitzone, automatische Antworten, Gebietsschema (Sprache und Land/Region) sowie Geschäftszeiten umfassen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-153">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="b0cd3-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="b0cd3-154">Response 1</span></span>
<span data-ttu-id="b0cd3-155">Die Antwort enthält alle postfacheinstellungen für das des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-155">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="b0cd3-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b0cd3-157">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-157">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
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
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="b0cd3-158">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="b0cd3-158">Request 2</span></span>
<span data-ttu-id="b0cd3-159">Im zweiten Beispiel werden die Einstellungen für automatische Antworten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-159">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="b0cd3-160">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="b0cd3-160">Response 2</span></span>
<span data-ttu-id="b0cd3-p109">Die Antwort enthält nur die Einstellungen für automatische Antworten. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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


##### <a name="request-3"></a><span data-ttu-id="b0cd3-164">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="b0cd3-164">Request 3</span></span>
<span data-ttu-id="b0cd3-165">Im dritten Beispiel werden die Einstellungen für die Geschäftszeiten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-165">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="b0cd3-166">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="b0cd3-166">Response 3</span></span>
<span data-ttu-id="b0cd3-167">Die Antwort enthält nur die Einstellungen für Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-167">The response includes only the working hours settings.</span></span> <span data-ttu-id="b0cd3-168">Beachten Sie, dass sich die Geschäftszeiten des Benutzers in einer [benutzerdefinierten Zeitzone](../resources/customtimezone.md) befinden.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-168">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="b0cd3-169">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b0cd3-170">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-170">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
