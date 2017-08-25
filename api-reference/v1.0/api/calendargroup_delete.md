# <a name="delete-calendargroup"></a><span data-ttu-id="4417d-101">CalendarGroup löschen</span><span class="sxs-lookup"><span data-stu-id="4417d-101">Delete calendarGroup</span></span>

<span data-ttu-id="4417d-102">Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="4417d-102">Delete a calendar group other than the default calendar group.</span></span>

<span data-ttu-id="4417d-p101">**Hinweis** Outlook.com unterstützt nur die Standardkalendergruppe, auf die über „/me/calendars“ zugegriffen werden kann. Sie können in Outlook.com keine Kalendergruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="4417d-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the /me/calendars shortcut. You cannot delete any calendar group in Outlook.com.</span></span>

## <a name="permissions"></a><span data-ttu-id="4417d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4417d-105">Permissions</span></span>
<span data-ttu-id="4417d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4417d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4417d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4417d-108">Permission type</span></span>      | <span data-ttu-id="4417d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4417d-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4417d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4417d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4417d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4417d-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="4417d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4417d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4417d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4417d-113">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="4417d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4417d-114">Application</span></span> | <span data-ttu-id="4417d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4417d-115">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4417d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4417d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4417d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4417d-117">Request headers</span></span>
| <span data-ttu-id="4417d-118">Name</span><span class="sxs-lookup"><span data-stu-id="4417d-118">Name</span></span>       | <span data-ttu-id="4417d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4417d-119">Type</span></span> | <span data-ttu-id="4417d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4417d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4417d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4417d-121">Authorization</span></span>  | <span data-ttu-id="4417d-122">string</span><span class="sxs-lookup"><span data-stu-id="4417d-122">string</span></span>  | <span data-ttu-id="4417d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4417d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4417d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4417d-125">Request body</span></span>
<span data-ttu-id="4417d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4417d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4417d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4417d-127">Response</span></span>

<span data-ttu-id="4417d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4417d-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4417d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4417d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4417d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4417d-131">Request</span></span>
<span data-ttu-id="4417d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4417d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="4417d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4417d-133">Response</span></span>
<span data-ttu-id="4417d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4417d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
