# <a name="delete-calendargroup"></a><span data-ttu-id="61544-101">CalendarGroup löschen</span><span class="sxs-lookup"><span data-stu-id="61544-101">Delete calendarGroup</span></span>

<span data-ttu-id="61544-102">Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="61544-102">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="61544-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61544-103">Permissions</span></span>

<span data-ttu-id="61544-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="61544-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61544-106">Permission type</span></span>                        | <span data-ttu-id="61544-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61544-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="61544-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61544-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="61544-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61544-109">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="61544-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61544-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61544-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61544-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="61544-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61544-112">Application</span></span>                            | <span data-ttu-id="61544-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61544-113">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="61544-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61544-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="61544-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61544-115">Request headers</span></span>

| <span data-ttu-id="61544-116">Name</span><span class="sxs-lookup"><span data-stu-id="61544-116">Name</span></span>          | <span data-ttu-id="61544-117">Typ</span><span class="sxs-lookup"><span data-stu-id="61544-117">Type</span></span>   | <span data-ttu-id="61544-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61544-118">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="61544-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="61544-119">Authorization</span></span> | <span data-ttu-id="61544-120">string</span><span class="sxs-lookup"><span data-stu-id="61544-120">string</span></span> | <span data-ttu-id="61544-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61544-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61544-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61544-123">Request body</span></span>

<span data-ttu-id="61544-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="61544-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61544-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="61544-125">Response</span></span>

<span data-ttu-id="61544-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61544-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61544-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61544-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61544-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61544-129">Request</span></span>

<span data-ttu-id="61544-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61544-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="61544-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="61544-131">Response</span></span>

<span data-ttu-id="61544-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61544-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
