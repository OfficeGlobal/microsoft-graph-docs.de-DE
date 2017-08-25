# <a name="delete-calendar"></a><span data-ttu-id="cd7f7-101">Kalender löschen</span><span class="sxs-lookup"><span data-stu-id="cd7f7-101">Delete calendar</span></span>

<span data-ttu-id="cd7f7-102">Mit dieser API können Sie Kalender löschen (nicht jedoch den Standardkalender).</span><span class="sxs-lookup"><span data-stu-id="cd7f7-102">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd7f7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd7f7-103">Permissions</span></span>
<span data-ttu-id="cd7f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd7f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd7f7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd7f7-106">Permission type</span></span>      | <span data-ttu-id="cd7f7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd7f7-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cd7f7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd7f7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cd7f7-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd7f7-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="cd7f7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd7f7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd7f7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd7f7-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="cd7f7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd7f7-112">Application</span></span> | <span data-ttu-id="cd7f7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd7f7-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cd7f7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd7f7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cd7f7-115">Ein anderer [Kalender](../resources/calendar.md) des Benutzers als der Standardkalender in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cd7f7-115">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="cd7f7-116">Ein anderer [Kalender](../resources/calendar.md) als der Standardkalender in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cd7f7-116">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cd7f7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd7f7-117">Request headers</span></span>
| <span data-ttu-id="cd7f7-118">Name</span><span class="sxs-lookup"><span data-stu-id="cd7f7-118">Name</span></span>           |  <span data-ttu-id="cd7f7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cd7f7-119">Type</span></span>    | <span data-ttu-id="cd7f7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd7f7-120">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="cd7f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd7f7-121">Authorization</span></span>  |  <span data-ttu-id="cd7f7-122">string</span><span class="sxs-lookup"><span data-stu-id="cd7f7-122">string</span></span>  | <span data-ttu-id="cd7f7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd7f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd7f7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd7f7-125">Request body</span></span>
<span data-ttu-id="cd7f7-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd7f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd7f7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd7f7-127">Response</span></span>

<span data-ttu-id="cd7f7-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd7f7-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd7f7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd7f7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd7f7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd7f7-131">Request</span></span>
<span data-ttu-id="cd7f7-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd7f7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="cd7f7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd7f7-133">Response</span></span>
<span data-ttu-id="cd7f7-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd7f7-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
