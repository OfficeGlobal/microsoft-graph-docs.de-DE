# <a name="update-calendar"></a><span data-ttu-id="97f02-101">Kalender aktualisieren</span><span class="sxs-lookup"><span data-stu-id="97f02-101">Update calendar</span></span>

<span data-ttu-id="97f02-102">Aktualisieren Sie die Eigenschaften eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97f02-102">Update the properties of calendar object.</span></span> <span data-ttu-id="97f02-103">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="97f02-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="97f02-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97f02-104">Permissions</span></span>
<span data-ttu-id="97f02-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97f02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97f02-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97f02-107">Permission type</span></span>      | <span data-ttu-id="97f02-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97f02-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f02-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97f02-109">Delegated (work or school account)</span></span> | <span data-ttu-id="97f02-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97f02-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="97f02-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97f02-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f02-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97f02-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="97f02-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97f02-113">Application</span></span> | <span data-ttu-id="97f02-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97f02-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f02-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97f02-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="97f02-116">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="97f02-116">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="97f02-117">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="97f02-117">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="97f02-118">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="97f02-118">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="97f02-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97f02-119">Request headers</span></span>
| <span data-ttu-id="97f02-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97f02-120">Header</span></span>       | <span data-ttu-id="97f02-121">Wert</span><span class="sxs-lookup"><span data-stu-id="97f02-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97f02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f02-122">Authorization</span></span>  | <span data-ttu-id="97f02-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97f02-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97f02-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97f02-125">Content-Type</span></span>  | <span data-ttu-id="97f02-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="97f02-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97f02-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97f02-128">Request body</span></span>
<span data-ttu-id="97f02-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="97f02-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97f02-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97f02-132">Property</span></span>     | <span data-ttu-id="97f02-133">Typ</span><span class="sxs-lookup"><span data-stu-id="97f02-133">Type</span></span>   |<span data-ttu-id="97f02-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f02-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97f02-135">color</span><span class="sxs-lookup"><span data-stu-id="97f02-135">color</span></span>|<span data-ttu-id="97f02-136">String</span><span class="sxs-lookup"><span data-stu-id="97f02-136">String</span></span>|<span data-ttu-id="97f02-p106">Gibt das Farbdesign an, um den Kalender von anderen Kalendern in einer Benutzeroberfläche zu unterscheiden. Die Eigenschaftswerte sind: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="97f02-p106">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="97f02-139">name</span><span class="sxs-lookup"><span data-stu-id="97f02-139">name</span></span>|<span data-ttu-id="97f02-140">String</span><span class="sxs-lookup"><span data-stu-id="97f02-140">String</span></span>|<span data-ttu-id="97f02-141">Der Kalendername.</span><span class="sxs-lookup"><span data-stu-id="97f02-141">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="97f02-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="97f02-142">Response</span></span>

<span data-ttu-id="97f02-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97f02-143">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97f02-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97f02-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97f02-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97f02-145">Request</span></span>
<span data-ttu-id="97f02-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97f02-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
##### <a name="response"></a><span data-ttu-id="97f02-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="97f02-147">Response</span></span>
<span data-ttu-id="97f02-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97f02-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
