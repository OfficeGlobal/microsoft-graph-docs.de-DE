# <a name="event-dismissreminder"></a><span data-ttu-id="f2f83-101">Ereignis: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="f2f83-101">event: dismissReminder</span></span>

<span data-ttu-id="f2f83-102">Schließen Sie eine Erinnerung, die für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="f2f83-102">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2f83-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2f83-103">Permissions</span></span>
<span data-ttu-id="f2f83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2f83-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2f83-106">Permission type</span></span>      | <span data-ttu-id="f2f83-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2f83-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f83-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2f83-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f83-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f83-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2f83-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2f83-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f83-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f83-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2f83-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2f83-112">Application</span></span> | <span data-ttu-id="f2f83-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f83-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f83-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2f83-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="f2f83-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2f83-115">Request headers</span></span>
| <span data-ttu-id="f2f83-116">Name</span><span class="sxs-lookup"><span data-stu-id="f2f83-116">Name</span></span>       | <span data-ttu-id="f2f83-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f2f83-117">Type</span></span> | <span data-ttu-id="f2f83-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2f83-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2f83-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f2f83-119">Authorization</span></span>  | <span data-ttu-id="f2f83-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2f83-120">string</span></span>  | <span data-ttu-id="f2f83-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2f83-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="f2f83-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2f83-123">Response</span></span>

<span data-ttu-id="f2f83-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2f83-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f83-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2f83-126">Example</span></span>

<span data-ttu-id="f2f83-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f2f83-127">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f2f83-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2f83-128">Request</span></span>
<span data-ttu-id="f2f83-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2f83-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="f2f83-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2f83-130">Response</span></span>
<span data-ttu-id="f2f83-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2f83-131">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
