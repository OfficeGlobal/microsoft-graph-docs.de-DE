# <a name="create-calendargroup"></a><span data-ttu-id="dc424-101">CalendarGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="dc424-101">Create CalendarGroup</span></span>

<span data-ttu-id="dc424-102">Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="dc424-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc424-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dc424-103">Permissions</span></span>
<span data-ttu-id="dc424-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc424-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dc424-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc424-106">Permission type</span></span>      | <span data-ttu-id="dc424-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc424-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc424-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc424-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dc424-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc424-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dc424-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc424-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc424-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc424-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dc424-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc424-112">Application</span></span> | <span data-ttu-id="dc424-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc424-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc424-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc424-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="dc424-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc424-115">Request headers</span></span>
| <span data-ttu-id="dc424-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dc424-116">Header</span></span>       | <span data-ttu-id="dc424-117">Wert</span><span class="sxs-lookup"><span data-stu-id="dc424-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc424-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc424-118">Authorization</span></span>  | <span data-ttu-id="dc424-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc424-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc424-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc424-121">Content-Type</span></span>  | <span data-ttu-id="dc424-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dc424-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc424-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc424-123">Request body</span></span>
<span data-ttu-id="dc424-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [CalendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="dc424-124">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dc424-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc424-125">Response</span></span>

<span data-ttu-id="dc424-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [CalendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc424-126">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc424-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc424-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc424-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc424-128">Request</span></span>
<span data-ttu-id="dc424-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc424-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="dc424-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="dc424-130">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dc424-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc424-131">Response</span></span>
<span data-ttu-id="dc424-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc424-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
