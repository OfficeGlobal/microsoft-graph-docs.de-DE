---
title: Postfacheinstellungen des Benutzers abrufen
description: 'Abrufen des Benutzers MailboxSettings. Einschließlich der Einstellungen für automatische Antworten (Personen automatisch beim Benachrichtigen '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e68d50cde270c20c76bce1e703ff07ff45c2107
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914563"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="58f3c-104">Postfacheinstellungen des Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="58f3c-104">Get user mailbox settings</span></span>

<span data-ttu-id="58f3c-p102">Rufen Sie die [mailboxSettings](../resources/mailboxsettings.md) des Benutzers ab. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema (Sprache und Land/Region), Zeitzone und die Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="58f3c-p102">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone, and working hours.</span></span>

<span data-ttu-id="58f3c-107">Sie können alle Postfacheinstellungen anzeigen oder bestimmte Einstellungen abrufen.</span><span class="sxs-lookup"><span data-stu-id="58f3c-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="58f3c-108">Zeitzone ist eine bevorzugte Einstellung, die ein Benutzer für das Benutzerpostfach einrichten kann.</span><span class="sxs-lookup"><span data-stu-id="58f3c-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="58f3c-109">Gültige Zeitzonenformate sind das Windows-Zeitzonenformat und das [IANA-Zeitzonenformat (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet).</span><span class="sxs-lookup"><span data-stu-id="58f3c-109">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="58f3c-110">Das Windows-Format ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="58f3c-110">The Windows format is the default.</span></span> 

<span data-ttu-id="58f3c-111">Wenn Sie die bevorzugte Zeitzone eines Benutzers abrufen, wird die Zeitzone in dem eingerichteten Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f3c-111">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="58f3c-112">Wenn Sie diese Zeitzone in einem bestimmten Format (Windows oder IANA) abrufen möchten, können Sie zunächst [die bevorzugte Zeitzone in das entsprechende Format als Postfacheinstellung ändern](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="58f3c-112">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="58f3c-113">Anschließend können Sie die Zeitzone in diesem Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="58f3c-113">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="58f3c-114">Alternativ können Sie die Formatkonvertierung separat in Ihrer App verwalten.</span><span class="sxs-lookup"><span data-stu-id="58f3c-114">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="58f3c-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58f3c-115">Permissions</span></span>
<span data-ttu-id="58f3c-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f3c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f3c-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58f3c-118">Permission type</span></span>      | <span data-ttu-id="58f3c-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58f3c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58f3c-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58f3c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="58f3c-121">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f3c-121">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="58f3c-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58f3c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58f3c-123">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f3c-123">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="58f3c-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58f3c-124">Application</span></span> | <span data-ttu-id="58f3c-125">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f3c-125">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58f3c-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58f3c-126">HTTP request</span></span>
<span data-ttu-id="58f3c-127">Alle postfacheinstellungen für einen Benutzer abrufen:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="58f3c-127">To get all mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="58f3c-128">Zum Abrufen von bestimmter Einstellungen - antwortet nur die automatische beispielsweise über Einstellungen, Gebietsschema, Zeitzone oder Arbeitszeit:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="58f3c-128">To get specific settings - for example, only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="58f3c-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="58f3c-129">Optional query parameters</span></span>
<span data-ttu-id="58f3c-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="58f3c-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="58f3c-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58f3c-131">Request headers</span></span>
| <span data-ttu-id="58f3c-132">Name</span><span class="sxs-lookup"><span data-stu-id="58f3c-132">Name</span></span>       | <span data-ttu-id="58f3c-133">Typ</span><span class="sxs-lookup"><span data-stu-id="58f3c-133">Type</span></span> | <span data-ttu-id="58f3c-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58f3c-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58f3c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f3c-135">Authorization</span></span>  | <span data-ttu-id="58f3c-136">string</span><span class="sxs-lookup"><span data-stu-id="58f3c-136">string</span></span>  | <span data-ttu-id="58f3c-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58f3c-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58f3c-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58f3c-139">Request body</span></span>
<span data-ttu-id="58f3c-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="58f3c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58f3c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="58f3c-141">Response</span></span>

<span data-ttu-id="58f3c-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eines der folgenden angeforderten Objekte im Antworttext zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="58f3c-142">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="58f3c-143">[mailboxSettings](../resources/mailboxsettings.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="58f3c-143">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="58f3c-144">[automaticRepliesSetting](../resources/automaticrepliessetting.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="58f3c-144">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="58f3c-145">[localeInfo](../resources/localeinfo.md)-Objekt</span><span class="sxs-lookup"><span data-stu-id="58f3c-145">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="58f3c-146">Zeichenfolge (für **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="58f3c-146">string (for **timeZone**)</span></span>
- [<span data-ttu-id="58f3c-147">workingHours</span><span class="sxs-lookup"><span data-stu-id="58f3c-147">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="58f3c-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58f3c-148">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="58f3c-149">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="58f3c-149">Request 1</span></span>
<span data-ttu-id="58f3c-150">Im ersten Beispiel werden alle Postfacheinstellungen des Postfachs des angemeldeten Benutzers abgerufen, die Einstellungen für Zeitzone, automatische Antworten, Gebietsschema (Sprache und Land/Region) sowie Geschäftszeiten umfassen.</span><span class="sxs-lookup"><span data-stu-id="58f3c-150">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="58f3c-151">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="58f3c-151">Response 1</span></span>
<span data-ttu-id="58f3c-p107">Die Antwort beinhaltet alle Postfacheinstellungen. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f3c-p107">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="58f3c-155">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="58f3c-155">Request 2</span></span>
<span data-ttu-id="58f3c-156">Im zweiten Beispiel werden die Einstellungen für automatische Antworten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="58f3c-156">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="58f3c-157">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="58f3c-157">Response 2</span></span>
<span data-ttu-id="58f3c-p108">Die Antwort enthält nur die Einstellungen für automatische Antworten. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f3c-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="58f3c-161">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="58f3c-161">Request 3</span></span>
<span data-ttu-id="58f3c-162">Im dritten Beispiel werden die Einstellungen für die Geschäftszeiten für das Postfach des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="58f3c-162">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="58f3c-163">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="58f3c-163">Response 3</span></span>
<span data-ttu-id="58f3c-164">Die Antwort enthält nur die Einstellungen für Geschäftszeiten.</span><span class="sxs-lookup"><span data-stu-id="58f3c-164">The response includes only the working hours settings.</span></span> <span data-ttu-id="58f3c-165">Beachten Sie, dass sich die Geschäftszeiten des Benutzers in einer [benutzerdefinierten Zeitzone](../resources/customtimezone.md) befinden.</span><span class="sxs-lookup"><span data-stu-id="58f3c-165">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="58f3c-166">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="58f3c-166">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="58f3c-167">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f3c-167">All of the properties will be returned from an actual call.</span></span>
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
