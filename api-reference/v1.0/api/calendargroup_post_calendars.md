# <a name="create-calendar"></a><span data-ttu-id="cd48d-101">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="cd48d-101">Create Calendar</span></span>

<span data-ttu-id="cd48d-102">Mit dieser API können Sie in einer Kalendergruppe einen neuen Kalender für einen [Benutzer](../resources/user.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="cd48d-102">Use this API to create a new Calendar in a calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="cd48d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd48d-103">Permissions</span></span>
<span data-ttu-id="cd48d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd48d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd48d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd48d-106">Permission type</span></span>      | <span data-ttu-id="cd48d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd48d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd48d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd48d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cd48d-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd48d-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cd48d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd48d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd48d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd48d-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cd48d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd48d-112">Application</span></span> | <span data-ttu-id="cd48d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd48d-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd48d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd48d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cd48d-115">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cd48d-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="cd48d-116">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cd48d-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="cd48d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd48d-117">Request headers</span></span>
| <span data-ttu-id="cd48d-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd48d-118">Header</span></span>       | <span data-ttu-id="cd48d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cd48d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd48d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd48d-120">Authorization</span></span>  | <span data-ttu-id="cd48d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd48d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd48d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd48d-123">Content-Type</span></span>  | <span data-ttu-id="cd48d-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="cd48d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd48d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd48d-126">Request body</span></span>
<span data-ttu-id="cd48d-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cd48d-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd48d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd48d-128">Response</span></span>

<span data-ttu-id="cd48d-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd48d-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd48d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd48d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd48d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd48d-131">Request</span></span>
<span data-ttu-id="cd48d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd48d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```
<span data-ttu-id="cd48d-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cd48d-133">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cd48d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd48d-134">Response</span></span>
<span data-ttu-id="cd48d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd48d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
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
