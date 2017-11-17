# <a name="section-copytonotebook"></a><span data-ttu-id="ab1b8-101">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="ab1b8-101">section: copyToNotebook</span></span>
<span data-ttu-id="ab1b8-102">Kopiert einen Abschnitt in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-102">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="ab1b8-103">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab1b8-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ab1b8-104">Permissions</span></span>
<span data-ttu-id="ab1b8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab1b8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab1b8-107">Permission type</span></span>      | <span data-ttu-id="ab1b8-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab1b8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab1b8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab1b8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ab1b8-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab1b8-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab1b8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab1b8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab1b8-112">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab1b8-112">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ab1b8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab1b8-113">Application</span></span> | <span data-ttu-id="ab1b8-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab1b8-114">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab1b8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab1b8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="ab1b8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab1b8-116">Request headers</span></span>
| <span data-ttu-id="ab1b8-117">Name</span><span class="sxs-lookup"><span data-stu-id="ab1b8-117">Name</span></span>       | <span data-ttu-id="ab1b8-118">Typ</span><span class="sxs-lookup"><span data-stu-id="ab1b8-118">Type</span></span> | <span data-ttu-id="ab1b8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab1b8-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab1b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab1b8-120">Authorization</span></span>  | <span data-ttu-id="ab1b8-121">string</span><span class="sxs-lookup"><span data-stu-id="ab1b8-121">string</span></span>  | <span data-ttu-id="ab1b8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab1b8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab1b8-124">Content-Type</span></span> | <span data-ttu-id="ab1b8-125">string</span><span class="sxs-lookup"><span data-stu-id="ab1b8-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ab1b8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab1b8-126">Request body</span></span>
<span data-ttu-id="ab1b8-127">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ab1b8-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="ab1b8-128">Parameter</span></span>    | <span data-ttu-id="ab1b8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ab1b8-129">Type</span></span>   |<span data-ttu-id="ab1b8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab1b8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab1b8-131">groupId</span><span class="sxs-lookup"><span data-stu-id="ab1b8-131">groupId</span></span>|<span data-ttu-id="ab1b8-132">String</span><span class="sxs-lookup"><span data-stu-id="ab1b8-132">String</span></span>|<span data-ttu-id="ab1b8-p103">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ab1b8-135">id</span><span class="sxs-lookup"><span data-stu-id="ab1b8-135">id</span></span>|<span data-ttu-id="ab1b8-136">String</span><span class="sxs-lookup"><span data-stu-id="ab1b8-136">String</span></span>|<span data-ttu-id="ab1b8-p104">Erforderlich. Die ID des Zielnotizbuchs.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p104">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="ab1b8-139">renameAs</span><span class="sxs-lookup"><span data-stu-id="ab1b8-139">renameAs</span></span>|<span data-ttu-id="ab1b8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab1b8-140">String</span></span>|<span data-ttu-id="ab1b8-p105">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="ab1b8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab1b8-143">Response</span></span>

<span data-ttu-id="ab1b8-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="ab1b8-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ab1b8-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab1b8-146">Example</span></span>
<span data-ttu-id="ab1b8-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab1b8-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab1b8-148">Request</span></span>
<span data-ttu-id="ab1b8-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="ab1b8-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab1b8-150">Response</span></span>
<span data-ttu-id="ab1b8-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ab1b8-151">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->