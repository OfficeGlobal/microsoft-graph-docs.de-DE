# <a name="create-event"></a><span data-ttu-id="65c04-101">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="65c04-101">Create Event</span></span>
<span data-ttu-id="65c04-102">Mit dieser API können Sie einen neuen [Termin](../resources/event.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="65c04-102">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65c04-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65c04-103">Permissions</span></span>
<span data-ttu-id="65c04-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65c04-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65c04-106">Permission type</span></span>      | <span data-ttu-id="65c04-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65c04-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65c04-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65c04-108">Delegated (work or school account)</span></span> | <span data-ttu-id="65c04-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65c04-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="65c04-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65c04-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65c04-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65c04-111">Not supported.</span></span>    |
|<span data-ttu-id="65c04-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65c04-112">Application</span></span> | <span data-ttu-id="65c04-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65c04-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65c04-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65c04-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="65c04-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65c04-115">Request headers</span></span>
| <span data-ttu-id="65c04-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="65c04-116">Header</span></span>       | <span data-ttu-id="65c04-117">Wert</span><span class="sxs-lookup"><span data-stu-id="65c04-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65c04-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="65c04-118">Authorization</span></span>  | <span data-ttu-id="65c04-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65c04-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65c04-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65c04-121">Request body</span></span>
<span data-ttu-id="65c04-122">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="65c04-122">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="65c04-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="65c04-123">Response</span></span>
<span data-ttu-id="65c04-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65c04-124">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65c04-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65c04-125">Example</span></span>
#### <a name="request"></a><span data-ttu-id="65c04-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65c04-126">Request</span></span>
<span data-ttu-id="65c04-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65c04-127">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="65c04-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="65c04-128">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="65c04-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="65c04-129">Response</span></span>
<span data-ttu-id="65c04-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65c04-130">Here is an example of the response.</span></span>
><span data-ttu-id="65c04-131">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="65c04-131">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65c04-132">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="65c04-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
