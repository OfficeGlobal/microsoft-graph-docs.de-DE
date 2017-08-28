# <a name="get-calendar"></a><span data-ttu-id="5295c-101">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="5295c-101">Get calendar</span></span>

<span data-ttu-id="5295c-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalenderobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="5295c-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5295c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5295c-103">Permissions</span></span>
<span data-ttu-id="5295c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5295c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5295c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5295c-106">Permission type</span></span>      | <span data-ttu-id="5295c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5295c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5295c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5295c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5295c-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5295c-109">Calendars.Read</span></span>    |
|<span data-ttu-id="5295c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5295c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5295c-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5295c-111">Calendars.Read</span></span>    |
|<span data-ttu-id="5295c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5295c-112">Application</span></span> | <span data-ttu-id="5295c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5295c-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5295c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5295c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5295c-115">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="5295c-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="5295c-116">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5295c-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="5295c-117">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5295c-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5295c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5295c-118">Optional query parameters</span></span>
<span data-ttu-id="5295c-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5295c-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5295c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5295c-120">Request headers</span></span>
| <span data-ttu-id="5295c-121">Name</span><span class="sxs-lookup"><span data-stu-id="5295c-121">Name</span></span>       | <span data-ttu-id="5295c-122">Typ</span><span class="sxs-lookup"><span data-stu-id="5295c-122">Type</span></span> | <span data-ttu-id="5295c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5295c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5295c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5295c-124">Authorization</span></span>  | <span data-ttu-id="5295c-125">string</span><span class="sxs-lookup"><span data-stu-id="5295c-125">string</span></span>  | <span data-ttu-id="5295c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5295c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5295c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5295c-128">Request body</span></span>
<span data-ttu-id="5295c-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5295c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5295c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5295c-130">Response</span></span>

<span data-ttu-id="5295c-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5295c-131">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5295c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5295c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5295c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5295c-133">Request</span></span>
<span data-ttu-id="5295c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5295c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="5295c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5295c-135">Response</span></span>
<span data-ttu-id="5295c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5295c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
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
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
