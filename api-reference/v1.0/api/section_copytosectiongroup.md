# <a name="section-copytosectiongroup"></a><span data-ttu-id="53a08-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="53a08-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="53a08-102">Kopiert einen Abschnitt in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="53a08-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="53a08-103">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="53a08-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53a08-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53a08-104">Prerequisites</span></span>
<span data-ttu-id="53a08-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="53a08-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="53a08-106">Notes.Create, Notes.ReadWrite oder Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a08-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="53a08-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53a08-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="53a08-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53a08-108">Request headers</span></span>
| <span data-ttu-id="53a08-109">Name</span><span class="sxs-lookup"><span data-stu-id="53a08-109">Name</span></span>       | <span data-ttu-id="53a08-110">Typ</span><span class="sxs-lookup"><span data-stu-id="53a08-110">Type</span></span> | <span data-ttu-id="53a08-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53a08-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53a08-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="53a08-112">Authorization</span></span>  | <span data-ttu-id="53a08-113">string</span><span class="sxs-lookup"><span data-stu-id="53a08-113">string</span></span>  | <span data-ttu-id="53a08-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53a08-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53a08-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53a08-116">Content-Type</span></span> | <span data-ttu-id="53a08-117">string</span><span class="sxs-lookup"><span data-stu-id="53a08-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="53a08-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53a08-118">Request body</span></span>
<span data-ttu-id="53a08-119">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="53a08-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="53a08-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="53a08-120">Parameter</span></span>    | <span data-ttu-id="53a08-121">Typ</span><span class="sxs-lookup"><span data-stu-id="53a08-121">Type</span></span>   |<span data-ttu-id="53a08-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53a08-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53a08-123">groupId</span><span class="sxs-lookup"><span data-stu-id="53a08-123">groupId</span></span>|<span data-ttu-id="53a08-124">String</span><span class="sxs-lookup"><span data-stu-id="53a08-124">String</span></span>|<span data-ttu-id="53a08-p102">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="53a08-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="53a08-127">id</span><span class="sxs-lookup"><span data-stu-id="53a08-127">id</span></span>|<span data-ttu-id="53a08-128">String</span><span class="sxs-lookup"><span data-stu-id="53a08-128">String</span></span>|<span data-ttu-id="53a08-p103">Erforderlich. Die ID der Zielabschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="53a08-p103">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="53a08-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="53a08-131">renameAs</span></span>|<span data-ttu-id="53a08-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53a08-132">String</span></span>|<span data-ttu-id="53a08-p104">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="53a08-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="53a08-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="53a08-135">Response</span></span>

<span data-ttu-id="53a08-p105">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="53a08-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="53a08-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53a08-138">Example</span></span>
<span data-ttu-id="53a08-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="53a08-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53a08-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53a08-140">Request</span></span>
<span data-ttu-id="53a08-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53a08-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="53a08-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="53a08-142">Response</span></span>
<span data-ttu-id="53a08-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53a08-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->