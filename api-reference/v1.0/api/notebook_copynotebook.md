# <a name="notebook-copynotebook"></a><span data-ttu-id="b975e-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="b975e-101">notebook: copyNotebook</span></span>
<span data-ttu-id="b975e-p101">Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="b975e-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="b975e-104">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="b975e-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b975e-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b975e-105">Prerequisites</span></span>
<span data-ttu-id="b975e-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="b975e-106">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="b975e-107">Notes.Create, Notes.ReadWrite oder Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b975e-107">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="b975e-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b975e-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="b975e-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b975e-109">Request headers</span></span>
| <span data-ttu-id="b975e-110">Name</span><span class="sxs-lookup"><span data-stu-id="b975e-110">Name</span></span>       | <span data-ttu-id="b975e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b975e-111">Type</span></span> | <span data-ttu-id="b975e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b975e-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b975e-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="b975e-113">Authorization</span></span>  | <span data-ttu-id="b975e-114">string</span><span class="sxs-lookup"><span data-stu-id="b975e-114">string</span></span>  | <span data-ttu-id="b975e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b975e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b975e-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b975e-117">Content-Type</span></span> | <span data-ttu-id="b975e-118">string</span><span class="sxs-lookup"><span data-stu-id="b975e-118">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b975e-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b975e-119">Request body</span></span>
<span data-ttu-id="b975e-p103">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt. Es ist in Ordnung, senden Sie einen leeren Text senden, wenn keine erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b975e-p103">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="b975e-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="b975e-122">Parameter</span></span>    | <span data-ttu-id="b975e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b975e-123">Type</span></span>   |<span data-ttu-id="b975e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b975e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b975e-125">groupId</span><span class="sxs-lookup"><span data-stu-id="b975e-125">groupId</span></span>|<span data-ttu-id="b975e-126">String</span><span class="sxs-lookup"><span data-stu-id="b975e-126">String</span></span>|<span data-ttu-id="b975e-p104">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="b975e-p104">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b975e-129">renameAs</span><span class="sxs-lookup"><span data-stu-id="b975e-129">renameAs</span></span>|<span data-ttu-id="b975e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b975e-130">String</span></span>|<span data-ttu-id="b975e-p105">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="b975e-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="b975e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b975e-133">Response</span></span>

<span data-ttu-id="b975e-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteOperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="b975e-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b975e-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b975e-136">Example</span></span>
<span data-ttu-id="b975e-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b975e-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b975e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b975e-138">Request</span></span>
<span data-ttu-id="b975e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b975e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="b975e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b975e-140">Response</span></span>
<span data-ttu-id="b975e-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b975e-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
