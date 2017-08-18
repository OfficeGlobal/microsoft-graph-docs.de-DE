# <a name="create-acceptedsender"></a><span data-ttu-id="cab36-101">acceptedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="cab36-101">Create acceptedSender</span></span>

<span data-ttu-id="cab36-102">Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="cab36-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="cab36-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der zulässigen Absender können Beiträge für Unterhaltungen der Gruppe bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cab36-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cab36-106">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="cab36-106">Prerequisites</span></span>
<span data-ttu-id="cab36-107">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="cab36-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="cab36-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cab36-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cab36-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cab36-109">Request headers</span></span>
| <span data-ttu-id="cab36-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cab36-110">Header</span></span>       | <span data-ttu-id="cab36-111">Wert</span><span class="sxs-lookup"><span data-stu-id="cab36-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cab36-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="cab36-112">Authorization</span></span>  | <span data-ttu-id="cab36-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cab36-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cab36-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cab36-115">Request body</span></span>
<span data-ttu-id="cab36-116">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="cab36-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="cab36-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="cab36-117">Response</span></span>

<span data-ttu-id="cab36-118">Diese Methode gibt den Antwortcode `204, No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cab36-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="cab36-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cab36-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cab36-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cab36-120">Request</span></span>
<span data-ttu-id="cab36-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cab36-121">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cab36-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="cab36-122">Response</span></span>
<span data-ttu-id="cab36-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cab36-123">Here is an example of the response.</span></span>
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
