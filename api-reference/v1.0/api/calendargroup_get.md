# <a name="get-calendargroup"></a><span data-ttu-id="6b654-101">CalendarGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="6b654-101">Get calendarGroup</span></span>

<span data-ttu-id="6b654-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="6b654-102">Retrieve the properties and relationships of a calendar group object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b654-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b654-103">Permissions</span></span>
<span data-ttu-id="6b654-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b654-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b654-106">Permission type</span></span>      | <span data-ttu-id="6b654-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b654-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b654-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b654-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6b654-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b654-109">Calendars.Read</span></span>    |
|<span data-ttu-id="6b654-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b654-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b654-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b654-111">Calendars.Read</span></span>    |
|<span data-ttu-id="6b654-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b654-112">Application</span></span> | <span data-ttu-id="6b654-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b654-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b654-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b654-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6b654-115">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6b654-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b654-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6b654-116">Optional query parameters</span></span>
<span data-ttu-id="6b654-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b654-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b654-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b654-118">Request headers</span></span>
| <span data-ttu-id="6b654-119">Name</span><span class="sxs-lookup"><span data-stu-id="6b654-119">Name</span></span>       | <span data-ttu-id="6b654-120">Typ</span><span class="sxs-lookup"><span data-stu-id="6b654-120">Type</span></span> | <span data-ttu-id="6b654-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b654-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b654-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b654-122">Authorization</span></span>  | <span data-ttu-id="6b654-123">string</span><span class="sxs-lookup"><span data-stu-id="6b654-123">string</span></span>  | <span data-ttu-id="6b654-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b654-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b654-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b654-126">Request body</span></span>
<span data-ttu-id="6b654-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b654-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b654-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b654-128">Response</span></span>

<span data-ttu-id="6b654-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b654-129">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b654-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b654-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b654-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b654-131">Request</span></span>
<span data-ttu-id="6b654-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b654-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="6b654-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b654-133">Response</span></span>
<span data-ttu-id="6b654-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b654-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
