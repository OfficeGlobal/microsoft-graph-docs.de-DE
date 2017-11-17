# <a name="create-rejectedsender"></a><span data-ttu-id="6efc7-101">rejectedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="6efc7-101">Create rejectedSender</span></span>

<span data-ttu-id="6efc7-102">Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="6efc7-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="6efc7-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im POST-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6efc7-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="6efc7-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6efc7-106">Permissions</span></span>
<span data-ttu-id="6efc7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6efc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6efc7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6efc7-109">Permission type</span></span>      | <span data-ttu-id="6efc7-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6efc7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6efc7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6efc7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6efc7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efc7-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6efc7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6efc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efc7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6efc7-114">Not supported.</span></span>    |
|<span data-ttu-id="6efc7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6efc7-115">Application</span></span> | <span data-ttu-id="6efc7-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efc7-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6efc7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6efc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6efc7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6efc7-118">Request headers</span></span>
| <span data-ttu-id="6efc7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6efc7-119">Header</span></span>       | <span data-ttu-id="6efc7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6efc7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6efc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efc7-121">Authorization</span></span>  | <span data-ttu-id="6efc7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6efc7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6efc7-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6efc7-124">Request body</span></span>
<span data-ttu-id="6efc7-125">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="6efc7-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="6efc7-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="6efc7-126">Response</span></span>

<span data-ttu-id="6efc7-127">Diese Methode gibt den Antwortcode `204 No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6efc7-127">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="6efc7-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6efc7-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6efc7-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6efc7-129">Request</span></span>
<span data-ttu-id="6efc7-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6efc7-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="6efc7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6efc7-131">Response</span></span>
<span data-ttu-id="6efc7-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6efc7-132">Here is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
