# <a name="event-tentativelyaccept"></a><span data-ttu-id="e39a7-101">Ereignis: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="e39a7-101">event: tentativelyAccept</span></span>

<span data-ttu-id="e39a7-102">Das angegebene [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) des Benutzers unter Vorbehalt annehmen.</span><span class="sxs-lookup"><span data-stu-id="e39a7-102">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e39a7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e39a7-103">Permissions</span></span>
<span data-ttu-id="e39a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e39a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e39a7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e39a7-106">Permission type</span></span>      | <span data-ttu-id="e39a7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e39a7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e39a7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e39a7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e39a7-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e39a7-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e39a7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e39a7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e39a7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e39a7-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e39a7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e39a7-112">Application</span></span> | <span data-ttu-id="e39a7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e39a7-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e39a7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39a7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="e39a7-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e39a7-115">Request headers</span></span>
| <span data-ttu-id="e39a7-116">Name</span><span class="sxs-lookup"><span data-stu-id="e39a7-116">Name</span></span>       | <span data-ttu-id="e39a7-117">Typ</span><span class="sxs-lookup"><span data-stu-id="e39a7-117">Type</span></span> | <span data-ttu-id="e39a7-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e39a7-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e39a7-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e39a7-119">Authorization</span></span>  | <span data-ttu-id="e39a7-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e39a7-120">string</span></span>  | <span data-ttu-id="e39a7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e39a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e39a7-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="e39a7-123">Content-Type</span></span> | <span data-ttu-id="e39a7-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e39a7-124">string</span></span>  | <span data-ttu-id="e39a7-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e39a7-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e39a7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e39a7-127">Request body</span></span>
<span data-ttu-id="e39a7-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e39a7-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e39a7-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="e39a7-129">Parameter</span></span>    | <span data-ttu-id="e39a7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e39a7-130">Type</span></span>   |<span data-ttu-id="e39a7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e39a7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e39a7-132">Kommentar</span><span class="sxs-lookup"><span data-stu-id="e39a7-132">comment</span></span>|<span data-ttu-id="e39a7-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e39a7-133">String</span></span>|<span data-ttu-id="e39a7-p104">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="e39a7-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="e39a7-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="e39a7-136">sendResponse</span></span>|<span data-ttu-id="e39a7-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e39a7-137">Boolean</span></span>|<span data-ttu-id="e39a7-p105">`true` ,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="e39a7-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="e39a7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39a7-141">Response</span></span>

<span data-ttu-id="e39a7-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e39a7-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e39a7-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e39a7-144">Example</span></span>
<span data-ttu-id="e39a7-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e39a7-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e39a7-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39a7-146">Request</span></span>
<span data-ttu-id="e39a7-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e39a7-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="e39a7-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39a7-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="e39a7-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39a7-149">Response</span></span>
<span data-ttu-id="e39a7-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e39a7-150">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
