# <a name="event-decline"></a><span data-ttu-id="2da0f-101">event: decline</span><span class="sxs-lookup"><span data-stu-id="2da0f-101">event: decline</span></span>

<span data-ttu-id="2da0f-102">Mit dieser API können Sie die Einladung zu dem angegebenen Ereignis löschen.</span><span class="sxs-lookup"><span data-stu-id="2da0f-102">Decline invitation to the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="2da0f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2da0f-103">Permissions</span></span>
<span data-ttu-id="2da0f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2da0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2da0f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2da0f-106">Permission type</span></span>      | <span data-ttu-id="2da0f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2da0f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2da0f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2da0f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2da0f-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da0f-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2da0f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2da0f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2da0f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da0f-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="2da0f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2da0f-112">Application</span></span> | <span data-ttu-id="2da0f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da0f-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2da0f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2da0f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline
POST /groups/{id}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline
POST /groups/{id}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```
## <a name="request-headers"></a><span data-ttu-id="2da0f-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2da0f-115">Request headers</span></span>
| <span data-ttu-id="2da0f-116">Name</span><span class="sxs-lookup"><span data-stu-id="2da0f-116">Name</span></span>       | <span data-ttu-id="2da0f-117">Typ</span><span class="sxs-lookup"><span data-stu-id="2da0f-117">Type</span></span> | <span data-ttu-id="2da0f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da0f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2da0f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da0f-119">Authorization</span></span>  | <span data-ttu-id="2da0f-120">string</span><span class="sxs-lookup"><span data-stu-id="2da0f-120">string</span></span>  | <span data-ttu-id="2da0f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2da0f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2da0f-123">Content-Type</span></span> | <span data-ttu-id="2da0f-124">string</span><span class="sxs-lookup"><span data-stu-id="2da0f-124">string</span></span>  | <span data-ttu-id="2da0f-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2da0f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2da0f-127">Request body</span></span>
<span data-ttu-id="2da0f-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2da0f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2da0f-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="2da0f-129">Parameter</span></span>    | <span data-ttu-id="2da0f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2da0f-130">Type</span></span>   |<span data-ttu-id="2da0f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da0f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2da0f-132">comment</span><span class="sxs-lookup"><span data-stu-id="2da0f-132">comment</span></span>|<span data-ttu-id="2da0f-133">String</span><span class="sxs-lookup"><span data-stu-id="2da0f-133">String</span></span>|<span data-ttu-id="2da0f-p104">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2da0f-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2da0f-136">sendResponse</span></span>|<span data-ttu-id="2da0f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da0f-137">Boolean</span></span>|<span data-ttu-id="2da0f-p105">`true`,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2da0f-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2da0f-141">Response</span></span>

<span data-ttu-id="2da0f-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2da0f-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da0f-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2da0f-144">Example</span></span>
<span data-ttu-id="2da0f-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2da0f-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2da0f-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2da0f-146">Request</span></span>
<span data-ttu-id="2da0f-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2da0f-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="2da0f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2da0f-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="2da0f-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="2da0f-149">Response</span></span>
<span data-ttu-id="2da0f-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2da0f-150">Here is an example of the response.</span></span>
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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
