# <a name="create-event"></a><span data-ttu-id="ac415-101">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="ac415-101">Create Event</span></span>

<span data-ttu-id="ac415-102">Verwenden Sie diese API zum Erstellen eines neuen [Ereignisses](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="ac415-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac415-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ac415-103">Prerequisites</span></span>
<span data-ttu-id="ac415-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ac415-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="ac415-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac415-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="ac415-106">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac415-106">Request headers</span></span>
| <span data-ttu-id="ac415-107">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac415-107">Header</span></span>       | <span data-ttu-id="ac415-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ac415-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac415-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac415-109">Authorization</span></span>  | <span data-ttu-id="ac415-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac415-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac415-112">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac415-112">Request body</span></span>
<span data-ttu-id="ac415-113">Geben Sie im Anforderungstext eine JSON-Darstellung des [Event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ac415-113">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ac415-114">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac415-114">Response</span></span>

<span data-ttu-id="ac415-115">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [Event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac415-115">If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac415-116">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac415-116">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac415-117">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac415-117">Request</span></span>
<span data-ttu-id="ac415-118">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac415-118">Here is an example of the request.</span></span>
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
<span data-ttu-id="ac415-119">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ac415-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ac415-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac415-120">Response</span></span>
<span data-ttu-id="ac415-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac415-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
