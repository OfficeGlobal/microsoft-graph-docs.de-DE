# <a name="create-acceptedsender"></a><span data-ttu-id="17231-101">acceptedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="17231-101">Create acceptedSender</span></span>

<span data-ttu-id="17231-102">Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="17231-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="17231-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der zulässigen Absender können Beiträge für Unterhaltungen der Gruppe bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="17231-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="17231-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="17231-106">Permissions</span></span>
<span data-ttu-id="17231-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="17231-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17231-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17231-109">Permission type</span></span>      | <span data-ttu-id="17231-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17231-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="17231-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17231-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17231-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17231-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="17231-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17231-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17231-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17231-114">Not supported.</span></span>    | 
|<span data-ttu-id="17231-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17231-115">Application</span></span> | <span data-ttu-id="17231-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17231-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="17231-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17231-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="17231-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17231-118">Request headers</span></span>
| <span data-ttu-id="17231-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="17231-119">Header</span></span>       | <span data-ttu-id="17231-120">Wert</span><span class="sxs-lookup"><span data-stu-id="17231-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17231-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17231-121">Authorization</span></span>  | <span data-ttu-id="17231-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17231-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17231-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17231-124">Request body</span></span>
<span data-ttu-id="17231-125">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="17231-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="17231-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="17231-126">Response</span></span>

<span data-ttu-id="17231-127">Diese Methode gibt den Antwortcode `204, No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="17231-127">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="17231-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17231-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17231-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17231-129">Request</span></span>
<span data-ttu-id="17231-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17231-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="17231-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="17231-131">Response</span></span>
<span data-ttu-id="17231-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="17231-132">Here is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
