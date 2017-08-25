# <a name="section-copytosectiongroup"></a><span data-ttu-id="fc12e-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="fc12e-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="fc12e-102">Kopiert einen Abschnitt in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fc12e-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="fc12e-103">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Aktion „Copy“ auf, und fragen Sie dann das Ergebnis vom Vorgangsendpunkt ab.</span><span class="sxs-lookup"><span data-stu-id="fc12e-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc12e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc12e-104">Permissions</span></span>
<span data-ttu-id="fc12e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc12e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc12e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc12e-107">Permission type</span></span>      | <span data-ttu-id="fc12e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc12e-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fc12e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc12e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fc12e-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc12e-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="fc12e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc12e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc12e-112">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc12e-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="fc12e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc12e-113">Application</span></span> | <span data-ttu-id="fc12e-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc12e-114">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fc12e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc12e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="fc12e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc12e-116">Request headers</span></span>
| <span data-ttu-id="fc12e-117">Name</span><span class="sxs-lookup"><span data-stu-id="fc12e-117">Name</span></span>       | <span data-ttu-id="fc12e-118">Typ</span><span class="sxs-lookup"><span data-stu-id="fc12e-118">Type</span></span> | <span data-ttu-id="fc12e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc12e-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc12e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc12e-120">Authorization</span></span>  | <span data-ttu-id="fc12e-121">string</span><span class="sxs-lookup"><span data-stu-id="fc12e-121">string</span></span>  | <span data-ttu-id="fc12e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc12e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc12e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc12e-124">Content-Type</span></span> | <span data-ttu-id="fc12e-125">string</span><span class="sxs-lookup"><span data-stu-id="fc12e-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fc12e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc12e-126">Request body</span></span>
<span data-ttu-id="fc12e-127">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="fc12e-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="fc12e-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="fc12e-128">Parameter</span></span>    | <span data-ttu-id="fc12e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fc12e-129">Type</span></span>   |<span data-ttu-id="fc12e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc12e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc12e-131">groupId</span><span class="sxs-lookup"><span data-stu-id="fc12e-131">groupId</span></span>|<span data-ttu-id="fc12e-132">String</span><span class="sxs-lookup"><span data-stu-id="fc12e-132">String</span></span>|<span data-ttu-id="fc12e-p103">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="fc12e-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="fc12e-135">id</span><span class="sxs-lookup"><span data-stu-id="fc12e-135">id</span></span>|<span data-ttu-id="fc12e-136">String</span><span class="sxs-lookup"><span data-stu-id="fc12e-136">String</span></span>|<span data-ttu-id="fc12e-p104">Erforderlich. Die ID der Zielabschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fc12e-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="fc12e-139">renameAs</span><span class="sxs-lookup"><span data-stu-id="fc12e-139">renameAs</span></span>|<span data-ttu-id="fc12e-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc12e-140">String</span></span>|<span data-ttu-id="fc12e-p105">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="fc12e-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="fc12e-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc12e-143">Response</span></span>

<span data-ttu-id="fc12e-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="fc12e-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="fc12e-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc12e-146">Example</span></span>
<span data-ttu-id="fc12e-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fc12e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc12e-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc12e-148">Request</span></span>
<span data-ttu-id="fc12e-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc12e-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="fc12e-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc12e-150">Response</span></span>
<span data-ttu-id="fc12e-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc12e-151">Here is an example of the response.</span></span>
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