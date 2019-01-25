---
title: 'user: reminderView'
description: 'Diese API gibt eine Liste von Kalendererinnerungen zurück, die im Zeitraum zwischen dem angegebenen Startdatum und dem angegebenen Enddatum liegen. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 34c2f1a55b6dea1daff36c5ce98d1959fd78b301
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510470"
---
# <a name="user-reminderview"></a><span data-ttu-id="8ca12-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="8ca12-103">user: reminderView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ca12-104">Eine Liste der Erinnerungen Ereignis in einem Benutzerkalender innerhalb der angegebenen Start- und Endzeiten zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="8ca12-104">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8ca12-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ca12-105">Permissions</span></span>
<span data-ttu-id="8ca12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ca12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ca12-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ca12-108">Permission type</span></span>      | <span data-ttu-id="8ca12-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ca12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ca12-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ca12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ca12-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca12-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8ca12-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ca12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ca12-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca12-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8ca12-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ca12-114">Application</span></span> | <span data-ttu-id="8ca12-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca12-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ca12-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ca12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="8ca12-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="8ca12-117">Function parameters</span></span>
<span data-ttu-id="8ca12-118">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="8ca12-118">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="8ca12-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="8ca12-119">Parameter</span></span>    | <span data-ttu-id="8ca12-120">Typ</span><span class="sxs-lookup"><span data-stu-id="8ca12-120">Type</span></span>   |<span data-ttu-id="8ca12-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ca12-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ca12-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8ca12-122">startDateTime</span></span>|<span data-ttu-id="8ca12-123">String</span><span class="sxs-lookup"><span data-stu-id="8ca12-123">String</span></span>|<span data-ttu-id="8ca12-p102">Das Startdatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="8ca12-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="8ca12-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8ca12-126">endDateTime</span></span>|<span data-ttu-id="8ca12-127">String</span><span class="sxs-lookup"><span data-stu-id="8ca12-127">String</span></span>|<span data-ttu-id="8ca12-p103">Das Enddatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="8ca12-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8ca12-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ca12-130">Request headers</span></span>
| <span data-ttu-id="8ca12-131">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8ca12-131">Header</span></span>       | <span data-ttu-id="8ca12-132">Wert</span><span class="sxs-lookup"><span data-stu-id="8ca12-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="8ca12-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ca12-133">Authorization</span></span>  | <span data-ttu-id="8ca12-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ca12-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ca12-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ca12-136">Content-Type</span></span>   | <span data-ttu-id="8ca12-137">application/json</span><span class="sxs-lookup"><span data-stu-id="8ca12-137">application/json</span></span> |
| <span data-ttu-id="8ca12-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="8ca12-138">Prefer</span></span> | <span data-ttu-id="8ca12-p105">{Time-zone}. Optional. Falls kein Wert vorhanden, wird UTC angenommen.</span><span class="sxs-lookup"><span data-stu-id="8ca12-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ca12-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ca12-141">Request body</span></span>
<span data-ttu-id="8ca12-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ca12-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ca12-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ca12-143">Response</span></span>

<span data-ttu-id="8ca12-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [reminder](../resources/reminder.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ca12-144">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca12-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ca12-145">Example</span></span>
<span data-ttu-id="8ca12-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8ca12-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8ca12-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ca12-147">Request</span></span>
<span data-ttu-id="8ca12-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ca12-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="8ca12-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ca12-149">Response</span></span>
<span data-ttu-id="8ca12-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ca12-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-reminderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
