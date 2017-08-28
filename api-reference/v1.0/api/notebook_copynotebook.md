# <a name="notebook-copynotebook"></a><span data-ttu-id="4a7c1-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="4a7c1-101">notebook: copyNotebook</span></span>
<span data-ttu-id="4a7c1-p101">Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="4a7c1-104">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a7c1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a7c1-105">Permissions</span></span>
<span data-ttu-id="4a7c1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a7c1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a7c1-108">Permission type</span></span>      | <span data-ttu-id="4a7c1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a7c1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a7c1-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7c1-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a7c1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a7c1-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a7c1-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4a7c1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a7c1-114">Application</span></span> | <span data-ttu-id="4a7c1-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7c1-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a7c1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a7c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="4a7c1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a7c1-117">Request headers</span></span>
| <span data-ttu-id="4a7c1-118">Name</span><span class="sxs-lookup"><span data-stu-id="4a7c1-118">Name</span></span>       | <span data-ttu-id="4a7c1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4a7c1-119">Type</span></span> | <span data-ttu-id="4a7c1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a7c1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a7c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a7c1-121">Authorization</span></span>  | <span data-ttu-id="4a7c1-122">string</span><span class="sxs-lookup"><span data-stu-id="4a7c1-122">string</span></span>  | <span data-ttu-id="4a7c1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a7c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a7c1-125">Content-Type</span></span> | <span data-ttu-id="4a7c1-126">string</span><span class="sxs-lookup"><span data-stu-id="4a7c1-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4a7c1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a7c1-127">Request body</span></span>
<span data-ttu-id="4a7c1-p104">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt. Es ist in Ordnung, senden Sie einen leeren Text senden, wenn keine erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p104">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="4a7c1-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="4a7c1-130">Parameter</span></span>    | <span data-ttu-id="4a7c1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4a7c1-131">Type</span></span>   |<span data-ttu-id="4a7c1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a7c1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a7c1-133">groupId</span><span class="sxs-lookup"><span data-stu-id="4a7c1-133">groupId</span></span>|<span data-ttu-id="4a7c1-134">String</span><span class="sxs-lookup"><span data-stu-id="4a7c1-134">String</span></span>|<span data-ttu-id="4a7c1-p105">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4a7c1-137">renameAs</span><span class="sxs-lookup"><span data-stu-id="4a7c1-137">renameAs</span></span>|<span data-ttu-id="4a7c1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a7c1-138">String</span></span>|<span data-ttu-id="4a7c1-p106">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p106">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="4a7c1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a7c1-141">Response</span></span>

<span data-ttu-id="4a7c1-p107">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteOperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4a7c1-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a7c1-144">Example</span></span>
<span data-ttu-id="4a7c1-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a7c1-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a7c1-146">Request</span></span>
<span data-ttu-id="4a7c1-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4a7c1-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a7c1-148">Response</span></span>
<span data-ttu-id="4a7c1-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-149">Here is an example of the response.</span></span>
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
