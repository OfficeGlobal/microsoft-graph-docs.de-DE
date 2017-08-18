# <a name="create-rejectedsender"></a><span data-ttu-id="998d2-101">rejectedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="998d2-101">Create rejectedSender</span></span>

<span data-ttu-id="998d2-102">Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="998d2-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="998d2-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im POST-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="998d2-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="998d2-106">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="998d2-106">Prerequisites</span></span>
<span data-ttu-id="998d2-107">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="998d2-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="998d2-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="998d2-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="998d2-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="998d2-109">Request headers</span></span>
| <span data-ttu-id="998d2-110">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="998d2-110">Header</span></span>       | <span data-ttu-id="998d2-111">Wert</span><span class="sxs-lookup"><span data-stu-id="998d2-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="998d2-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="998d2-112">Authorization</span></span>  | <span data-ttu-id="998d2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="998d2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="998d2-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="998d2-115">Request body</span></span>
<span data-ttu-id="998d2-116">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="998d2-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="998d2-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="998d2-117">Response</span></span>

<span data-ttu-id="998d2-118">Diese Methode gibt den Antwortcode `204, No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="998d2-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="998d2-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="998d2-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="998d2-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="998d2-120">Request</span></span>
<span data-ttu-id="998d2-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="998d2-121">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="998d2-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="998d2-122">Response</span></span>
<span data-ttu-id="998d2-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="998d2-123">Here is an example of the response.</span></span>
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
