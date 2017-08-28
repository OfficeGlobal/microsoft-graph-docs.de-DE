# <a name="event-snoozereminder"></a><span data-ttu-id="74d9b-101">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="74d9b-101">event: snoozeReminder</span></span>

<span data-ttu-id="74d9b-102">Mit dieser API können Sie eine Erinnerung auf einen neuen Termin verschieben.</span><span class="sxs-lookup"><span data-stu-id="74d9b-102">Postpone a reminder until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="74d9b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74d9b-103">Permissions</span></span>
<span data-ttu-id="74d9b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="74d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74d9b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74d9b-106">Permission type</span></span>      | <span data-ttu-id="74d9b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74d9b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74d9b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74d9b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="74d9b-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74d9b-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="74d9b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74d9b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d9b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74d9b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="74d9b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74d9b-112">Application</span></span> | <span data-ttu-id="74d9b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74d9b-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74d9b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74d9b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder
POST /groups/{id}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder
POST /groups/{id}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="74d9b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74d9b-115">Request headers</span></span>
| <span data-ttu-id="74d9b-116">Name</span><span class="sxs-lookup"><span data-stu-id="74d9b-116">Name</span></span>       | <span data-ttu-id="74d9b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="74d9b-117">Type</span></span> | <span data-ttu-id="74d9b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74d9b-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74d9b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d9b-119">Authorization</span></span>  | <span data-ttu-id="74d9b-120">string</span><span class="sxs-lookup"><span data-stu-id="74d9b-120">string</span></span>  | <span data-ttu-id="74d9b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74d9b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74d9b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74d9b-123">Content-Type</span></span> | <span data-ttu-id="74d9b-124">string</span><span class="sxs-lookup"><span data-stu-id="74d9b-124">string</span></span>  | <span data-ttu-id="74d9b-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74d9b-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74d9b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74d9b-127">Request body</span></span>
<span data-ttu-id="74d9b-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="74d9b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74d9b-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="74d9b-129">Parameter</span></span>    | <span data-ttu-id="74d9b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="74d9b-130">Type</span></span>   |<span data-ttu-id="74d9b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74d9b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74d9b-132">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="74d9b-132">newReminderTime</span></span>|<span data-ttu-id="74d9b-133">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="74d9b-133">DateTimeTimeZone</span></span>|<span data-ttu-id="74d9b-134">Das neue Datum und die neue Uhrzeit für die Auslösung der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="74d9b-134">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="74d9b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="74d9b-135">Response</span></span>

<span data-ttu-id="74d9b-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74d9b-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74d9b-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74d9b-138">Example</span></span>
<span data-ttu-id="74d9b-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="74d9b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74d9b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74d9b-140">Request</span></span>
<span data-ttu-id="74d9b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74d9b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="74d9b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="74d9b-142">Response</span></span>
<span data-ttu-id="74d9b-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74d9b-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
