---
title: Postfacheinstellungen des Benutzers aktualisieren
description: Aktualisieren Sie eine oder mehrere Einstellungen des Postfachs des Benutzers. Dies umfasst die Einstellungen für automatische Antworten (automatische Benachrichtigung von Personen über den Empfang von E-Mails), Gebietsschema (Sprache und Land/Region), Zeitzone und die Geschäftszeiten.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90140a5c6f7822730b172dbc5a424c97b2fafc39
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516224"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="40d43-104">Postfacheinstellungen des Benutzers aktualisieren</span><span class="sxs-lookup"><span data-stu-id="40d43-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40d43-p102">Aktualisieren Sie eine oder mehrere Einstellungen des Postfachs des Benutzers. Dies umfasst die Einstellungen für [automatische Antworten](../resources/automaticrepliessetting.md) (automatische Benachrichtigung von Personen über den Empfang von E-Mails), [Gebietsschema](../resources/localeinfo.md) (Sprache und Land/Region), Zeitzone und die [Geschäftszeiten](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="40d43-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="40d43-107">Diese Einstellungen können Sie im Rahmen des [mailboxSettings](../resources/mailboxsettings.md)-Elements aktivieren, konfigurieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="40d43-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="40d43-108">**Hinweis:** Sie können keine Postfacheinstellungen erstellen oder löschen.</span><span class="sxs-lookup"><span data-stu-id="40d43-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="40d43-109">Wenn Sie die bevorzugte Zeitzone für einen Benutzer aktualisieren, können Sie diese im Windows- oder im [IANA-Format](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet) angeben.</span><span class="sxs-lookup"><span data-stu-id="40d43-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="40d43-110">Sie können die Zeitzone auch weiter anpassen, wie in [Beispiel 2](#request-2) weiter unten dargestellt.</span><span class="sxs-lookup"><span data-stu-id="40d43-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="40d43-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40d43-111">Permissions</span></span>
<span data-ttu-id="40d43-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d43-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40d43-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40d43-114">Permission type</span></span>      | <span data-ttu-id="40d43-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40d43-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40d43-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40d43-116">Delegated (work or school account)</span></span> | <span data-ttu-id="40d43-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40d43-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="40d43-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40d43-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d43-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40d43-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="40d43-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40d43-120">Application</span></span> | <span data-ttu-id="40d43-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40d43-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d43-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40d43-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40d43-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="40d43-123">Optional query parameters</span></span>
<span data-ttu-id="40d43-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40d43-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40d43-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40d43-125">Request headers</span></span>
| <span data-ttu-id="40d43-126">Name</span><span class="sxs-lookup"><span data-stu-id="40d43-126">Name</span></span>       | <span data-ttu-id="40d43-127">Typ</span><span class="sxs-lookup"><span data-stu-id="40d43-127">Type</span></span> | <span data-ttu-id="40d43-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d43-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40d43-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="40d43-129">Authorization</span></span>  | <span data-ttu-id="40d43-130">string</span><span class="sxs-lookup"><span data-stu-id="40d43-130">string</span></span>  | <span data-ttu-id="40d43-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40d43-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40d43-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40d43-133">Request body</span></span>
<span data-ttu-id="40d43-p106">Geben Sie im Anforderungstext die Werte für die relevanten Eigenschaften an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Im Folgenden werden die beschreibbaren/aktualisierbaren Eigenschaften aufgelistet:</span><span class="sxs-lookup"><span data-stu-id="40d43-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="40d43-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40d43-138">Property</span></span>     | <span data-ttu-id="40d43-139">Typ</span><span class="sxs-lookup"><span data-stu-id="40d43-139">Type</span></span>   |<span data-ttu-id="40d43-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d43-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40d43-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="40d43-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="40d43-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="40d43-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="40d43-143">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="40d43-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="40d43-144">Sie können solche Benachrichtigungen für nur einen zukünftigen Datumsbereich festlegen.</span><span class="sxs-lookup"><span data-stu-id="40d43-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="40d43-145">language</span><span class="sxs-lookup"><span data-stu-id="40d43-145">language</span></span>|[<span data-ttu-id="40d43-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="40d43-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="40d43-147">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="40d43-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="40d43-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="40d43-148">timeZone</span></span>|<span data-ttu-id="40d43-149">string</span><span class="sxs-lookup"><span data-stu-id="40d43-149">string</span></span>|<span data-ttu-id="40d43-150">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40d43-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="40d43-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="40d43-151">workingHours</span></span>|[<span data-ttu-id="40d43-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="40d43-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="40d43-153">Die Stunden, Wochentage und die Zeitzone, an denen bzw. in der der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="40d43-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="40d43-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="40d43-154">Response</span></span>

<span data-ttu-id="40d43-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [mailboxSettings](../resources/mailboxsettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d43-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="40d43-156">Fehler</span><span class="sxs-lookup"><span data-stu-id="40d43-156">Errors</span></span>

<span data-ttu-id="40d43-157">Durch Festlegen von Geschäftszeiten mit falschen Werten können möglicherweise die folgenden Fehler zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="40d43-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="40d43-158">Szenario</span><span class="sxs-lookup"><span data-stu-id="40d43-158">Scenario</span></span>   | <span data-ttu-id="40d43-159">HTTP-Statuscode</span><span class="sxs-lookup"><span data-stu-id="40d43-159">HTTP status code</span></span> | <span data-ttu-id="40d43-160">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="40d43-160">Error code</span></span> | <span data-ttu-id="40d43-161">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="40d43-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="40d43-162">Ungültige **startTime** oder **endTime**</span><span class="sxs-lookup"><span data-stu-id="40d43-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="40d43-163">400</span><span class="sxs-lookup"><span data-stu-id="40d43-163">400</span></span> | <span data-ttu-id="40d43-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="40d43-164">RequestBodyRead</span></span> | <span data-ttu-id="40d43-165">Das Literal „08“ kann nicht in den erwarteten Typ „Edm.TimeOfDay“ konvertiert werden.</span><span class="sxs-lookup"><span data-stu-id="40d43-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="40d43-166">Die Startzeit größer als die Endzeit</span><span class="sxs-lookup"><span data-stu-id="40d43-166">Start time is greater than end time</span></span> | <span data-ttu-id="40d43-167">400</span><span class="sxs-lookup"><span data-stu-id="40d43-167">400</span></span> | <span data-ttu-id="40d43-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="40d43-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="40d43-169">Die Startzeit muss vor der Endzeit liegen.</span><span class="sxs-lookup"><span data-stu-id="40d43-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="40d43-170">Ungültiger Tag in **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="40d43-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="40d43-171">400</span><span class="sxs-lookup"><span data-stu-id="40d43-171">400</span></span> | <span data-ttu-id="40d43-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="40d43-172">InvalidArguments</span></span> | <span data-ttu-id="40d43-173">Der angeforderte Wert „RandomDay“ wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="40d43-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="40d43-174">Ungültige **timeZone**</span><span class="sxs-lookup"><span data-stu-id="40d43-174">Invalid **timeZone**</span></span> | <span data-ttu-id="40d43-175">400</span><span class="sxs-lookup"><span data-stu-id="40d43-175">400</span></span> | <span data-ttu-id="40d43-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="40d43-176">InvalidTimeZone</span></span> | <span data-ttu-id="40d43-177">Die angegebenen Zeitzoneneinstellungen sind ungültig.</span><span class="sxs-lookup"><span data-stu-id="40d43-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="40d43-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d43-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="40d43-179">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="40d43-179">Request 1</span></span>
<span data-ttu-id="40d43-180">Im folgenden Beispiel werden automatische Antworten für einen bestimmten Datumsbereich durch Festlegen der folgenden Eigenschaften der **automaticRepliesSetting**-Eigenschaft aktiviert: **status**, **scheduledStartDateTime** und **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="40d43-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
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
##### <a name="response-1"></a><span data-ttu-id="40d43-181">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="40d43-181">Response 1</span></span>
<span data-ttu-id="40d43-182">Die Antwort enthält die aktualisierten Einstellungen für automatische Antworten.</span><span class="sxs-lookup"><span data-stu-id="40d43-182">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="40d43-183">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="40d43-183">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="40d43-184">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d43-184">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
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
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="40d43-185">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="40d43-185">Request 2</span></span>
<span data-ttu-id="40d43-186">Das zweite Beispiel passt die Zeitzone für die Geschäftszeiten des angemeldeten Benutzers an, indem die **timeZone**-Eigenschaft auf eine [benutzerdefinierte Zeitzone](../resources/customtimezone.md) festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="40d43-186">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a><span data-ttu-id="40d43-187">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="40d43-187">Response 2</span></span>
<span data-ttu-id="40d43-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d43-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
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
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-mailboxsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
