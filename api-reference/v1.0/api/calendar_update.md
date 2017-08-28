# <a name="update-calendar"></a><span data-ttu-id="474df-101">Kalender aktualisieren</span><span class="sxs-lookup"><span data-stu-id="474df-101">Update calendar</span></span>

<span data-ttu-id="474df-102">Mit dieser API können Sie die Eigenschaften eines Kalenderobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="474df-102">Update the properties of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="474df-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="474df-103">Permissions</span></span>
<span data-ttu-id="474df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="474df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="474df-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="474df-106">Permission type</span></span>      | <span data-ttu-id="474df-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="474df-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="474df-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="474df-108">Delegated (work or school account)</span></span> | <span data-ttu-id="474df-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474df-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="474df-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="474df-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="474df-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474df-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="474df-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="474df-112">Application</span></span> | <span data-ttu-id="474df-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474df-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="474df-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="474df-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="474df-115">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="474df-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="474df-116">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="474df-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="474df-117">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="474df-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="474df-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="474df-118">Request headers</span></span>
| <span data-ttu-id="474df-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="474df-119">Header</span></span>       | <span data-ttu-id="474df-120">Wert</span><span class="sxs-lookup"><span data-stu-id="474df-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="474df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="474df-121">Authorization</span></span>  | <span data-ttu-id="474df-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="474df-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="474df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="474df-124">Content-Type</span></span>  | <span data-ttu-id="474df-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="474df-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="474df-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="474df-127">Request body</span></span>
<span data-ttu-id="474df-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="474df-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="474df-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="474df-131">Property</span></span>     | <span data-ttu-id="474df-132">Typ</span><span class="sxs-lookup"><span data-stu-id="474df-132">Type</span></span>   |<span data-ttu-id="474df-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="474df-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="474df-134">color</span><span class="sxs-lookup"><span data-stu-id="474df-134">color</span></span>|<span data-ttu-id="474df-135">String</span><span class="sxs-lookup"><span data-stu-id="474df-135">String</span></span>|<span data-ttu-id="474df-p105">Gibt das Farbdesign an, um den Kalender von anderen Kalendern in einer Benutzeroberfläche zu unterscheiden. Die Eigenschaftswerte sind: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="474df-p105">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="474df-138">name</span><span class="sxs-lookup"><span data-stu-id="474df-138">name</span></span>|<span data-ttu-id="474df-139">String</span><span class="sxs-lookup"><span data-stu-id="474df-139">String</span></span>|<span data-ttu-id="474df-140">Der Kalendername.</span><span class="sxs-lookup"><span data-stu-id="474df-140">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="474df-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="474df-141">Response</span></span>

<span data-ttu-id="474df-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="474df-142">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="474df-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="474df-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="474df-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="474df-144">Request</span></span>
<span data-ttu-id="474df-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="474df-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="474df-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="474df-146">Response</span></span>
<span data-ttu-id="474df-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="474df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
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
