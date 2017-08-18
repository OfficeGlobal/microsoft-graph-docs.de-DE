# <a name="create-calendar"></a><span data-ttu-id="071d6-101">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="071d6-101">Create Calendar</span></span>

<span data-ttu-id="071d6-102">Verwenden Sie diese API zum Erstellen eines neuen Kalenders.</span><span class="sxs-lookup"><span data-stu-id="071d6-102">Use this API to create a new calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="071d6-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="071d6-103">Prerequisites</span></span>
<span data-ttu-id="071d6-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="071d6-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="071d6-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="071d6-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="071d6-106">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="071d6-106">Request headers</span></span>
| <span data-ttu-id="071d6-107">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="071d6-107">Header</span></span>       | <span data-ttu-id="071d6-108">Wert</span><span class="sxs-lookup"><span data-stu-id="071d6-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="071d6-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="071d6-109">Authorization</span></span>  | <span data-ttu-id="071d6-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="071d6-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="071d6-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="071d6-112">Content-Type</span></span>  | <span data-ttu-id="071d6-113">application/json</span><span class="sxs-lookup"><span data-stu-id="071d6-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="071d6-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="071d6-114">Request body</span></span>
<span data-ttu-id="071d6-115">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="071d6-115">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="071d6-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="071d6-116">Response</span></span>

<span data-ttu-id="071d6-117">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="071d6-117">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="071d6-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="071d6-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="071d6-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="071d6-119">Request</span></span>
<span data-ttu-id="071d6-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="071d6-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="071d6-121">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="071d6-121">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="071d6-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="071d6-122">Response</span></span>
<span data-ttu-id="071d6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="071d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
