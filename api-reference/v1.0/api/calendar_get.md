# <a name="get-calendar"></a><span data-ttu-id="fcfad-101">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="fcfad-101">Get calendar</span></span>

<span data-ttu-id="fcfad-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fcfad-102">Retrieve the properties and relationships of a calendar group object.</span></span> <span data-ttu-id="fcfad-103">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="fcfad-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="fcfad-104">Abrufen des Kalenders eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="fcfad-104">Get another user's calendar</span></span>

<span data-ttu-id="fcfad-105">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie den Kalender eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="fcfad-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="fcfad-106">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="fcfad-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="fcfad-107">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="fcfad-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="fcfad-108">Der Benutzer Garth hat einen Kalender für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="fcfad-108">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="fcfad-109">Sie können den freigegebenen Kalender aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="fcfad-109">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="fcfad-110">Diese Funktion gilt für alle unterstützten GET-Kalendervorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="fcfad-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="fcfad-111">Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="fcfad-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="fcfad-112">Wenn Garth weder seinen Kalender für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcfad-112">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="fcfad-113">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um den Kalender eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="fcfad-113">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="fcfad-114">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="fcfad-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="fcfad-115">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="fcfad-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="fcfad-116">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="fcfad-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="fcfad-117">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="fcfad-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="fcfad-118">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="fcfad-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="fcfad-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fcfad-119">Permissions</span></span>
<span data-ttu-id="fcfad-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcfad-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcfad-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fcfad-122">Permission type</span></span>      | <span data-ttu-id="fcfad-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fcfad-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcfad-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fcfad-124">Delegated (work or school account)</span></span> | <span data-ttu-id="fcfad-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcfad-125">Calendars.Read</span></span>    |
|<span data-ttu-id="fcfad-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fcfad-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcfad-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcfad-127">Calendars.Read</span></span>    |
|<span data-ttu-id="fcfad-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fcfad-128">Application</span></span> | <span data-ttu-id="fcfad-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcfad-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcfad-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcfad-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fcfad-131">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="fcfad-131">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="fcfad-132">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="fcfad-132">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="fcfad-133">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="fcfad-133">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fcfad-134">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fcfad-134">Optional query parameters</span></span>
<span data-ttu-id="fcfad-135">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fcfad-135">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fcfad-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fcfad-136">Request headers</span></span>
| <span data-ttu-id="fcfad-137">Name</span><span class="sxs-lookup"><span data-stu-id="fcfad-137">Name</span></span>       | <span data-ttu-id="fcfad-138">Typ</span><span class="sxs-lookup"><span data-stu-id="fcfad-138">Type</span></span> | <span data-ttu-id="fcfad-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcfad-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcfad-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcfad-140">Authorization</span></span>  | <span data-ttu-id="fcfad-141">string</span><span class="sxs-lookup"><span data-stu-id="fcfad-141">string</span></span>  | <span data-ttu-id="fcfad-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fcfad-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcfad-144">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fcfad-144">Request body</span></span>
<span data-ttu-id="fcfad-145">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fcfad-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcfad-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcfad-146">Response</span></span>

<span data-ttu-id="fcfad-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcfad-147">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fcfad-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fcfad-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcfad-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcfad-149">Request</span></span>
<span data-ttu-id="fcfad-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fcfad-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="fcfad-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcfad-151">Response</span></span>
<span data-ttu-id="fcfad-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcfad-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
