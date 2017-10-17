# <a name="event-decline"></a><span data-ttu-id="86d18-101">event: decline</span><span class="sxs-lookup"><span data-stu-id="86d18-101">event: decline</span></span>

<span data-ttu-id="86d18-102">Mit dieser API können Sie die Einladung zu dem angegebenen Ereignis löschen.</span><span class="sxs-lookup"><span data-stu-id="86d18-102">Decline invitation to the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="86d18-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86d18-103">Permissions</span></span>

<span data-ttu-id="86d18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86d18-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86d18-106">Permission type</span></span>      | <span data-ttu-id="86d18-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86d18-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86d18-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86d18-108">Delegated (work or school account)</span></span> | <span data-ttu-id="86d18-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d18-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86d18-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86d18-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86d18-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d18-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86d18-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86d18-112">Application</span></span> | <span data-ttu-id="86d18-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d18-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="86d18-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d18-114">HTTP request</span></span>

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

<br/>

## <a name="request-headers"></a><span data-ttu-id="86d18-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86d18-115">Request headers</span></span>

| <span data-ttu-id="86d18-116">Name</span><span class="sxs-lookup"><span data-stu-id="86d18-116">Name</span></span>       | <span data-ttu-id="86d18-117">Typ</span><span class="sxs-lookup"><span data-stu-id="86d18-117">Type</span></span> | <span data-ttu-id="86d18-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86d18-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86d18-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d18-119">Authorization</span></span>  | <span data-ttu-id="86d18-120">string</span><span class="sxs-lookup"><span data-stu-id="86d18-120">string</span></span>  | <span data-ttu-id="86d18-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86d18-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86d18-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86d18-123">Content-Type</span></span> | <span data-ttu-id="86d18-124">string</span><span class="sxs-lookup"><span data-stu-id="86d18-124">string</span></span>  | <span data-ttu-id="86d18-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86d18-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86d18-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86d18-127">Request body</span></span>

<span data-ttu-id="86d18-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="86d18-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="86d18-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="86d18-129">Parameter</span></span>    | <span data-ttu-id="86d18-130">Typ</span><span class="sxs-lookup"><span data-stu-id="86d18-130">Type</span></span>   |<span data-ttu-id="86d18-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86d18-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86d18-132">comment</span><span class="sxs-lookup"><span data-stu-id="86d18-132">comment</span></span>|<span data-ttu-id="86d18-133">String</span><span class="sxs-lookup"><span data-stu-id="86d18-133">String</span></span>|<span data-ttu-id="86d18-p104">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="86d18-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="86d18-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="86d18-136">sendResponse</span></span>|<span data-ttu-id="86d18-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="86d18-137">Boolean</span></span>|<span data-ttu-id="86d18-p105">`true`,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="86d18-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="86d18-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="86d18-141">Response</span></span>

<span data-ttu-id="86d18-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86d18-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86d18-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86d18-144">Example</span></span>

<span data-ttu-id="86d18-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="86d18-145">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="86d18-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d18-146">Request</span></span>

<span data-ttu-id="86d18-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86d18-147">Here is an example of the request.</span></span>

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

<br/>

### <a name="response"></a><span data-ttu-id="86d18-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="86d18-148">Response</span></span>

<span data-ttu-id="86d18-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86d18-149">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
