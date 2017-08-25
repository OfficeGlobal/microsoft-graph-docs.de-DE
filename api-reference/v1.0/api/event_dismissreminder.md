# <a name="event-dismissreminder"></a><span data-ttu-id="1ab15-101">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="1ab15-101">event: dismissReminder</span></span>

<span data-ttu-id="1ab15-102">Mit dieser API können Sie eine ausgelöste Erinnerung schließen.</span><span class="sxs-lookup"><span data-stu-id="1ab15-102">Dissmiss a reminder that has been triggered.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ab15-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ab15-103">Permissions</span></span>
<span data-ttu-id="1ab15-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ab15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ab15-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ab15-106">Permission type</span></span>      | <span data-ttu-id="1ab15-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ab15-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1ab15-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ab15-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1ab15-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ab15-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="1ab15-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ab15-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab15-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ab15-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="1ab15-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ab15-112">Application</span></span> | <span data-ttu-id="1ab15-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ab15-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1ab15-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ab15-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder
POST /groups/{id}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder
POST /groups/{id}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```
## <a name="request-headers"></a><span data-ttu-id="1ab15-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ab15-115">Request headers</span></span>
| <span data-ttu-id="1ab15-116">Name</span><span class="sxs-lookup"><span data-stu-id="1ab15-116">Name</span></span>       | <span data-ttu-id="1ab15-117">Typ</span><span class="sxs-lookup"><span data-stu-id="1ab15-117">Type</span></span> | <span data-ttu-id="1ab15-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ab15-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ab15-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ab15-119">Authorization</span></span>  | <span data-ttu-id="1ab15-120">string</span><span class="sxs-lookup"><span data-stu-id="1ab15-120">string</span></span>  | <span data-ttu-id="1ab15-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ab15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ab15-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ab15-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1ab15-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ab15-124">Response</span></span>

<span data-ttu-id="1ab15-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ab15-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ab15-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ab15-127">Example</span></span>
<span data-ttu-id="1ab15-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1ab15-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1ab15-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ab15-129">Request</span></span>
<span data-ttu-id="1ab15-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ab15-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

##### <a name="response"></a><span data-ttu-id="1ab15-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ab15-131">Response</span></span>
##### <a name="response"></a><span data-ttu-id="1ab15-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ab15-132">Response</span></span>
<span data-ttu-id="1ab15-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1ab15-133">Here is an example of the response.</span></span>
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
