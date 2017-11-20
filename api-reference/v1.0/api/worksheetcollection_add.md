# <a name="worksheetcollection-add"></a><span data-ttu-id="2e7f0-101">WorksheetCollection: Hinzufügen</span><span class="sxs-lookup"><span data-stu-id="2e7f0-101">WorksheetCollection: add</span></span>

<span data-ttu-id="2e7f0-p101">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblättern hinzugefügt. Wenn Sie das neu hinzugefügte Arbeitsblatt aktivieren möchten, rufen Sie „.activate()“ dazu auf.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e7f0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e7f0-105">Permissions</span></span>
<span data-ttu-id="2e7f0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e7f0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e7f0-108">Permission type</span></span>      | <span data-ttu-id="2e7f0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e7f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e7f0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e7f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e7f0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e7f0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e7f0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e7f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e7f0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e7f0-113">Not supported.</span></span>    |
|<span data-ttu-id="2e7f0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e7f0-114">Application</span></span> | <span data-ttu-id="2e7f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e7f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e7f0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e7f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="2e7f0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e7f0-117">Request headers</span></span>
| <span data-ttu-id="2e7f0-118">Name</span><span class="sxs-lookup"><span data-stu-id="2e7f0-118">Name</span></span>       | <span data-ttu-id="2e7f0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e7f0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e7f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e7f0-120">Authorization</span></span>  | <span data-ttu-id="2e7f0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e7f0-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2e7f0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e7f0-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e7f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e7f0-126">Request body</span></span>
<span data-ttu-id="2e7f0-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e7f0-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="2e7f0-128">Parameter</span></span>    | <span data-ttu-id="2e7f0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2e7f0-129">Type</span></span>   |<span data-ttu-id="2e7f0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e7f0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e7f0-131">name</span><span class="sxs-lookup"><span data-stu-id="2e7f0-131">name</span></span>|<span data-ttu-id="2e7f0-132">string</span><span class="sxs-lookup"><span data-stu-id="2e7f0-132">string</span></span>|<span data-ttu-id="2e7f0-p105">Optional. Der Name des hinzuzufügenden Arbeitsblatts. Falls angegeben, sollte der Name eindeutig sein. Falls nicht angegeben, bestimmt Excel den Namen des neuen Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="2e7f0-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e7f0-137">Response</span></span>

<span data-ttu-id="2e7f0-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Worksheet](../resources/worksheet.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-138">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e7f0-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e7f0-139">Example</span></span>
<span data-ttu-id="2e7f0-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2e7f0-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e7f0-141">Request</span></span>
<span data-ttu-id="2e7f0-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="2e7f0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e7f0-143">Response</span></span>
<span data-ttu-id="2e7f0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e7f0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->