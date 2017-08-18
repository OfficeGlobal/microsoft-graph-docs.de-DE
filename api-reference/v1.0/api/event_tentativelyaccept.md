# <a name="event-tentativelyaccept"></a><span data-ttu-id="0decc-101">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="0decc-101">event: tentativelyAccept</span></span>

<span data-ttu-id="0decc-102">Dient zum Annehmen des angegebenen Ereignisses mit Vorbehalt.</span><span class="sxs-lookup"><span data-stu-id="0decc-102">Tentatively accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0decc-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0decc-103">Prerequisites</span></span>
<span data-ttu-id="0decc-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="0decc-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="0decc-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0decc-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept
POST /groups/{id}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept
POST /groups/{id}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="0decc-106">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0decc-106">Request headers</span></span>
| <span data-ttu-id="0decc-107">Name</span><span class="sxs-lookup"><span data-stu-id="0decc-107">Name</span></span>       | <span data-ttu-id="0decc-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0decc-108">Type</span></span> | <span data-ttu-id="0decc-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0decc-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0decc-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="0decc-110">Authorization</span></span>  | <span data-ttu-id="0decc-111">string</span><span class="sxs-lookup"><span data-stu-id="0decc-111">string</span></span>  | <span data-ttu-id="0decc-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0decc-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0decc-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0decc-114">Content-Type</span></span> | <span data-ttu-id="0decc-115">string</span><span class="sxs-lookup"><span data-stu-id="0decc-115">string</span></span>  | <span data-ttu-id="0decc-p102">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0decc-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0decc-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0decc-118">Request body</span></span>
<span data-ttu-id="0decc-119">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0decc-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0decc-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="0decc-120">Parameter</span></span>    | <span data-ttu-id="0decc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0decc-121">Type</span></span>   |<span data-ttu-id="0decc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0decc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0decc-123">comment</span><span class="sxs-lookup"><span data-stu-id="0decc-123">comment</span></span>|<span data-ttu-id="0decc-124">String</span><span class="sxs-lookup"><span data-stu-id="0decc-124">String</span></span>|<span data-ttu-id="0decc-p103">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="0decc-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="0decc-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="0decc-127">sendResponse</span></span>|<span data-ttu-id="0decc-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0decc-128">Boolean</span></span>|<span data-ttu-id="0decc-p104">`true`, wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="0decc-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="0decc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0decc-132">Response</span></span>

<span data-ttu-id="0decc-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0decc-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0decc-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0decc-135">Example</span></span>
<span data-ttu-id="0decc-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0decc-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0decc-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0decc-137">Request</span></span>
<span data-ttu-id="0decc-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0decc-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0decc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0decc-139">Response</span></span>
##### <a name="response"></a><span data-ttu-id="0decc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0decc-140">Response</span></span>
<span data-ttu-id="0decc-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0decc-141">Here is an example of the response.</span></span>
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
