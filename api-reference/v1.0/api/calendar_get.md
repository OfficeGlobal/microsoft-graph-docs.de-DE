# <a name="get-calendar"></a><span data-ttu-id="01bb0-101">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="01bb0-101">Get calendar</span></span>

<span data-ttu-id="01bb0-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="01bb0-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="01bb0-103">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="01bb0-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="01bb0-104">Es gibt zwei Szenarien, in denen eine App den Kalender eines anderen Benutzers abrufen kann:</span><span class="sxs-lookup"><span data-stu-id="01bb0-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="01bb0-105">Wenn die App über Anwendungsberechtigungen verfügt, oder</span><span class="sxs-lookup"><span data-stu-id="01bb0-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="01bb0-106">Wenn die App über die entsprechenden delegierten [Berechtigungen](#permissions) von einem Benutzer verfügt und ein anderer Benutzer einen Kalender für diesen Benutzer freigegeben hat oder delegierten Zugriff auf diesen Benutzer gewährt hat.</span><span class="sxs-lookup"><span data-stu-id="01bb0-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="01bb0-107">Siehe [Details und ein Beispiel](../../../concepts/outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="01bb0-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01bb0-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="01bb0-108">Permissions</span></span>
<span data-ttu-id="01bb0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01bb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01bb0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01bb0-111">Permission type</span></span>      | <span data-ttu-id="01bb0-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01bb0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01bb0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01bb0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="01bb0-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bb0-114">Calendars.Read</span></span>    |
|<span data-ttu-id="01bb0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01bb0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01bb0-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bb0-116">Calendars.Read</span></span>    |
|<span data-ttu-id="01bb0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01bb0-117">Application</span></span> | <span data-ttu-id="01bb0-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bb0-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="01bb0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01bb0-119">HTTP request</span></span>
<span data-ttu-id="01bb0-120"><!-- { "blockType": "ignored" } --> Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="01bb0-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="01bb0-121">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="01bb0-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="01bb0-122">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="01bb0-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01bb0-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="01bb0-123">Optional query parameters</span></span>
<span data-ttu-id="01bb0-124">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="01bb0-124">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01bb0-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01bb0-125">Request headers</span></span>
| <span data-ttu-id="01bb0-126">Name</span><span class="sxs-lookup"><span data-stu-id="01bb0-126">Name</span></span>       | <span data-ttu-id="01bb0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="01bb0-127">Type</span></span> | <span data-ttu-id="01bb0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01bb0-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01bb0-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="01bb0-129">Authorization</span></span>  | <span data-ttu-id="01bb0-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01bb0-130">string</span></span>  | <span data-ttu-id="01bb0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01bb0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01bb0-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01bb0-133">Request body</span></span>
<span data-ttu-id="01bb0-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="01bb0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01bb0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="01bb0-135">Response</span></span>

<span data-ttu-id="01bb0-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01bb0-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01bb0-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01bb0-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01bb0-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01bb0-138">Request</span></span>
<span data-ttu-id="01bb0-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01bb0-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="01bb0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="01bb0-140">Response</span></span>
<span data-ttu-id="01bb0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01bb0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
