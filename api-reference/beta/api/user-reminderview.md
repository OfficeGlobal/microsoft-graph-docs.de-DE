---
title: 'user: reminderView'
description: 'Diese API gibt eine Liste von Kalendererinnerungen zurück, die im Zeitraum zwischen dem angegebenen Startdatum und dem angegebenen Enddatum liegen. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fb0283aaae4f814f06b59a8a6ad6183cc18fec1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918210"
---
# <a name="user-reminderview"></a><span data-ttu-id="99cbe-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="99cbe-103">user: reminderView</span></span>

> <span data-ttu-id="99cbe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99cbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99cbe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99cbe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99cbe-106">Eine Liste der Erinnerungen Ereignis in einem Benutzerkalender innerhalb der angegebenen Start- und Endzeiten zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="99cbe-106">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="99cbe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99cbe-107">Permissions</span></span>
<span data-ttu-id="99cbe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99cbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99cbe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99cbe-110">Permission type</span></span>      | <span data-ttu-id="99cbe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99cbe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99cbe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99cbe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99cbe-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99cbe-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="99cbe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99cbe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99cbe-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99cbe-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="99cbe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99cbe-116">Application</span></span> | <span data-ttu-id="99cbe-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99cbe-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99cbe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99cbe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="99cbe-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="99cbe-119">Function parameters</span></span>
<span data-ttu-id="99cbe-120">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="99cbe-120">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="99cbe-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="99cbe-121">Parameter</span></span>    | <span data-ttu-id="99cbe-122">Typ</span><span class="sxs-lookup"><span data-stu-id="99cbe-122">Type</span></span>   |<span data-ttu-id="99cbe-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99cbe-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99cbe-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99cbe-124">startDateTime</span></span>|<span data-ttu-id="99cbe-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99cbe-125">String</span></span>|<span data-ttu-id="99cbe-p103">Das Startdatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p103">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="99cbe-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="99cbe-128">endDateTime</span></span>|<span data-ttu-id="99cbe-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99cbe-129">String</span></span>|<span data-ttu-id="99cbe-p104">Das Enddatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p104">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="99cbe-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99cbe-132">Request headers</span></span>
| <span data-ttu-id="99cbe-133">Header</span><span class="sxs-lookup"><span data-stu-id="99cbe-133">Header</span></span>       | <span data-ttu-id="99cbe-134">Wert</span><span class="sxs-lookup"><span data-stu-id="99cbe-134">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="99cbe-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="99cbe-135">Authorization</span></span>  | <span data-ttu-id="99cbe-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99cbe-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99cbe-138">Content-Type</span></span>   | <span data-ttu-id="99cbe-139">application/json</span><span class="sxs-lookup"><span data-stu-id="99cbe-139">application/json</span></span> |
| <span data-ttu-id="99cbe-140">Prefer</span><span class="sxs-lookup"><span data-stu-id="99cbe-140">Prefer</span></span> | <span data-ttu-id="99cbe-p106">{Time-zone}. Optional. Falls kein Wert vorhanden, wird UTC angenommen.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p106">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99cbe-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99cbe-143">Request body</span></span>
<span data-ttu-id="99cbe-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="99cbe-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99cbe-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="99cbe-145">Response</span></span>

<span data-ttu-id="99cbe-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [reminder](../resources/reminder.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99cbe-146">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99cbe-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99cbe-147">Example</span></span>
<span data-ttu-id="99cbe-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="99cbe-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99cbe-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99cbe-149">Request</span></span>
<span data-ttu-id="99cbe-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99cbe-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="99cbe-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="99cbe-151">Response</span></span>
<span data-ttu-id="99cbe-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
